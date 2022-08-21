[21 AUG 2022]()

# URIs
Unique Resource Identifiers(URIs) are used to address resources in the Rest APIs. 

**Good Example:**
http://api.example.restapi.org/france/paris/louvre/leonardo-da-vinci/mona-lisa

**Bad Example(Hard to understand Example):**
http://api.example.restapi.org/fd343-ds34-jjh-jjhjkdsf-4343j33434

Rest API Designers should design the URI such a way so that client can understand about resource just by looking at the URI.

# URI Format
URI = scheme “://” authority “/” path [ “?” query ] [ “#” fragment ]

**Rule: Forward slash separator (/) must be used to indicate a hierarchical relationship
**
http://api.canvas.restapi.org/shapes/polygons/quadrilaterals/squares

**Rule: A trailing forward slash(/) should not be included in URIs.**

http://api.canvas.restapi.org/shapes/ - Incorrect

http://api.canvas.restapi.org/shapes - Correct

Slash(/) should only be used when you want to represent some hierarchy between the resources. Unnecessarily don’t use it, as it doesn’t add any value.

**Rule: Hyphens(-) Should be used to improve the readability of URIs.**

http://api.canvas.restapi.org/blogs/mark-masse/entries/this-is-my-first-post

**Rule: Underscore(_) should not be used in URIs**

It’s because, usually text viewers applications like (browsers, editors etc..) often underline URIs to provide a visual cue that they are clickable. So in that case there is a chance that _ can’t be visible while reading the URL, so it’s better to avoid it.

**Rule: Lowercase Letters should be preferred in URI Paths**

URIs are case-sensitive except for the scheme and host components

1.  http://api.example.restapi.org/my-folder/my-doc
2.  http://API.EXAMPLE.RESTAPI.ORG/my-folder/my-doc
3. http://api.example.restapi.org/My-folder/my-doc


URI 1 and 2 are similar and represent the same resource. URI 3 isn't the same as 1 and 2, it doesn't represent the same resource.

**Rule: File extensions should not be included in URIs**

A REST API should not include artificial file extensions in URIs to indicate the format of a message’s entire body. Instead, they should rely on the media type, as communicated through the Content-Type header.

1. http://api.college.restapi.org/students/343434343/transcripts/fall.json
2. http://api.college.restapi.org/students/343434343/transcripts/fall

URI 1 should n’t be used to indicate format preference

URI 2 is the correct format, with the content type of the resource specified in the header.
