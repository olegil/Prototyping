'''csharp
@using Prototyping.Ipsum;
@using Prototyping.Placeholdit;
//Ipsum examples //Random paragraph
@Html.Ipsum()
//Paragraph
@Html.Ipsum().p()
//Four paragraphs, ten sentences
@Html.Ipsum().p(4, 10)
//Paragraph with the attribute class="fancy"
@Html.Ipsum().p(htmlAttributes: new { @class = "fancy" })
//h1 tag
@Html.Ipsum().h1()
//h1 tag, just one word long
@Html.Ipsum().h1(1)
//h2 tag, with the attribute data-special="true"
@Html.Ipsum().h2(5, new { data_special = "true" })
//unordered list
@Html.Ipsum().ul()
//unordered list of links
@Html.Ipsum().ul(links: true)
//a mock blog post
@Html.Ipsum().BlogPost()
//non HTML ipsum
@Html.Ipsum().Words(50)
@Html.Ipsum().Paragraphs(2)
//Fluent api
@Html.Ipsum().h1().p().h2().p().h3().ol(10,3, true)
//Image placeholder
@Html.Placehold(300,300)
'''