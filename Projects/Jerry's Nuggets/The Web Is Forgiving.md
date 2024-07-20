# The Web Is Forgiving

*A study in rethinking constraints* 

## On designing the Web

When he was inventing the World Wide Web (without VC funding or likely any thought that it would rapidly span the world), Tim Berners-Lee made many clever architectural decisions. 

For example, he needed a way to standardize document formats so that they looked the same however you accessed them, from whatever device you were using. Inventing a document format would've been a large project in and of itself, but there was already a standard called [SGML](http://en.wikipedia.org/wiki/Standard_Generalized_Markup_Language), the Standard Generalized Markup Language.

But SGML was expensive, cumbersome, and (most importantly here) strict: if a document's creator made any mistake in the document, it wouldn't compile. They had to fix all the errors in a document until they had a perfect document. Then they could use it.

None of those flaws was going to help Tim's fledgling Web fly. So he created a stripped-down version of SGML that he called HTML, the HyperText Markup Language. HTML had many fewer variables and options than SGML, which made it far less complete, but much easier to manage. Then the magic feature: the "browser" he created to receive and present HTML documents was *forgiving*. 

 A cool feature of HTML documents is that they can include component parts from anywhere around the Web. An image doesn't need to be on the same server where the main HTML body is; it can be on any other server on the planet. These days, ads, Captchas, payment widgets and other newer features can also come from arbitrarily distant Web services.

It's your Web browser's job to collect all the incoming parts, assemble them per the instructions in HTML, and present them to you. When you resize the browser window, the text and images flow around and adapt. You're so familiar with these features that you take them completely for granted.

Here's where forgiveness comes in: If one of those many pieces of content didn't arrive, the Wed browser would just substitute it with an icon of a broken component, and carry on. The webpage would still render with everything else that it did get. 

![[Broken-image-icon-in-Chrome.gif]]
## Rethinking Constraints

