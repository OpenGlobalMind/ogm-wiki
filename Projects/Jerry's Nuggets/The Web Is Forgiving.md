# The Web Is Forgiving

*A study in rethinking constraints* 

## On designing the Web

When he was inventing the World Wide Web (without VC funding or likely any thought that it would so rapidly span the world), Tim Berners-Lee made many clever architectural decisions. 

For example, he needed a way to standardize document formats so that they looked the same however you accessed them, from whatever device you were using. Inventing a document format would've been a large project in and of itself, but there was already a standard called [SGML](http://en.wikipedia.org/wiki/Standard_Generalized_Markup_Language), the Standard Generalized Markup Language.

But SGML was expensive, cumbersome, and (most importantly here) strict: if a document's creator made any mistake in the document, it wouldn't compile. The creator had to fix all the errors in a document until they had a perfect document. Then they could use it.

None of those flaws was going to help Tim's fledgling Web fly. So he created a stripped-down version of SGML that he called HTML, the HyperText Markup Language. HTML had many fewer variables and options than SGML, which made it far less complete, but much easier to manage, and less expensive to implement. Then the magic feature: the "browser" he created to receive and present HTML documents was *forgiving*. 

A little background: A cool feature of HTML documents is that they can include component parts from anywhere around the Web. An image doesn't need to be on the same server where the main HTML body is; it can be on any other server on the planet. These days, ads, Captchas, payment widgets and other features can also come from distributed Web services.

It's your Web browser's job to collect all the incoming parts, assemble them per the instructions in HTML, and present them to you. When you resize the browser window, the text and images flow around and adapt. You're so familiar with these features that you take them completely for granted.

Here's where forgiveness comes in: If one of those many pieces of content didn't arrive, the Web browser would just substitute it with an icon of a broken component, and carry on. The webpage would still render with everything else that it did get. 

![[Broken-image-icon-in-Chrome.gif]]
## Rethinking Constraints

*This is the first in what will likely be many posts about rethinking constraints.* 

I love stories like this. Stories of people finding solutions by questioning conventional wisdom, by poking at — then flipping — the status quo. That's the spirit of rethinking constraints. 

Berners-Lee understood the constraints that kept SGML from being more broadly useful, and found a way past them. It took a creative leap to think differently from the developers of SGML and its related applications. SGML was complicated because it could do so much. It was robust for industry applications like documentation for the US Department of Defense. What it wasn't is flexible and light. Or forgiving.

But "forgiving" wasn't on anyones requirements list. In fact, graceful degradation runs against most project goals, which seek six-sigma quality (meaning very low error rates) or very complete functionality. 

This post is cross-posted on [Substack](https://rethinkconstraints.substack.com/p/the-web-is-forgiving) and [LinkedIn](https://www.linkedin.com/pulse/web-forgiving-jerry-michalski-7udjc). [[On Cross-Posting]]. 