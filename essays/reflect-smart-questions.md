---
layout: essay
type: essay
title: "Asking Smart Questions"
# All dates must be YYYY-MM-DD format!
date: 2023-09-07
published: true
labels:
  - StackOverflow
---

In order to learn the most about a subject, you have to ask questions. But the quality of the questions is more important than the quantity. Constantly asking an expert on a subject simple yes or no questions isn't the most efficient way to learn, and it will make your learning journey much longer than it needs to be. In the age of the internet, asking smart questions is even more important. Having access to vast amounts of information is useless if you can't ask the right questions. 

## So how do you ask a smart question online?

<img width="500px" src="../img/reflect-smart-questions/logo-stackoverflow.png">

A smart question is one that makes it clear what you are looking to learn. If you are looking to learn how to do something, you want to make it clear from the beginning what your goal is. 

This example of a smart question comes from Stack Overflow, a website made to ask questions about programming.

```
Q: Sort array of objects by string property value

I have an array of JavaScript objects:

var objs = [ 
    { first_nom: 'Lazslo', last_nom: 'Jamf'     },
    { first_nom: 'Pig',    last_nom: 'Bodine'   },
    { first_nom: 'Pirate', last_nom: 'Prentice' }
];

How can I sort them by the value of last_nom in JavaScript?

I know about sort(a,b), but that only seems to work on strings and numbers. Do I need to add a toString() method to my objects?
```
Source: <a href="https://stackoverflow.com/questions/1129216/sort-array-of-objects-by-string-property-value"><i class="large github icon "></i>stackoverflow.com/questions/1129216/sort-array-of-objects-by-string-property-value</a>

Here, this user is asking about how to sort an array of objects based on a specific string property. The title of the question is brief, and clearly asks what they are looking to learn. Furthermore, they provide a simple example of the situation where the solution they are looking for could be used. This makes it clear to both potential answerers and other people with the same question what is being asked. They also provide additional context in telling other solutions they have attempted, and ask about a lead to the solution that they thought of.

This question recieved 4050 upvotes and 60 people provided an answer. While this is likely because the question is a common one, it is also because the question was asked in a smart way.

## If there are smart questions, does that mean there are stupid questions?

While teachers will commonly encourage students to ask questions by saying there are "no stupid questions", there certainly are ways to ask questions in a "stupid" or not smart way.

Here is another example from Stack Overflow.


```
Q: How can i do this in c#

question updated: for clarification, sorry if my question is not clear.

here we go. what im trying to do here is change the tag name of a spefic tag based on its attribute, and delete the attribute

in this example i need to change Emphasis name with attribute italic to i tag name, and para textbreak="no" to p tag

here is how i populate my listview

    //add data to listview
                this.lvContent.Items.Add(new MyItem { Tag = "Emphasis", Attribute = "Type", Value = "Italic", NewTag = "i" });
                this.lvContent.Items.Add(new MyItem { Tag = "Para", Attribute = "TextBreak", Value = "No", NewTag = "p" });


            foreach (MyItem item in lvContent.Items)
            {

                XElement rootI = XElement.Parse(txtInput.Text);
                IEnumerable<XElement> Emphasis =
                    from el in rootI.Descendants("" + item.Tag + "")
                    where (string)el.Attribute("" + item.Attribute + "") == "" + item.Value + ""
                    select el;

                foreach (XElement el in Emphasis)
                {
                    el.Name = "" + item.NewTag + "";
                }

                XElement xdoc = XElement.Parse(rootI.ToString());
                var elementsToRemove = from elemet in xdoc.Descendants(item.NewTag)
                                       where elemet.Attribute(item.Attribute).Value == item.Value
                                       select elemet;
                foreach (var ee in elementsToRemove)
                {
                    if (ee.Attribute(item.Attribute).Value == item.Value)
                    {
                        ee.RemoveAttributes();
                    }
                }
                Console.WriteLine(xdoc.ToString());
}
the output of the program

<Abstract>
  <Heading>Abstract</Heading>
  <Para TextBreak="No">Some paragraph <i>q</i></Para>
</Abstract>
<Abstract>
  <Heading>Abstract</Heading>
  <p>Some paragraph <Emphasis Type="Italic">q</Emphasis></p>
</Abstract>
and this is the correct output

<Abstract>
  <Heading>Abstract</Heading>
  <p>Some paragraph <i>q</i></p>
</Abstract>
the reason im asking how to pass the output of the first loop to the next loop is to

be used as INPUT to the next loop is because of the output.

i hope my question is clear now.
```
Source: 

<a href="https://stackoverflow.com/questions/38473176/how-can-i-do-this-in-c-sharp"><i class="large github icon "></i>https://stackoverflow.com/questions/38473176/how-can-i-do-this-in-c-sharp</a>

To start, the title of the question does not make it clear what the person is looking to learn. All any potential answerer is prompted with is how to do what they want to do in the programming language C#. By the time I found this question, it had already been edited to be made more clear what the person was looking for.

Even after editing however, the problem that they are looking to solve is not clear. At the top of their post, they ask how to change the name of a tag based on its attribute, then delete that attribute. Yet at the end of their post, they ask how to pass the output of one loop into another loop. It is unclear exactly what their goal is with this program. Even though their question is unclear, the example they provide helps to clarify their problem. It shows what they are trying to do, the incorrect output they are receiving, and the goal output. But that saving grace alone is not enough to make this a smart question.

This question was asked over 7 years ago, and has seen 4 answers. But, none of the answers were what the user was looking for. All of the answers provided were given before they updated their question, meaning that after they clarified their question, nobody else attempted to provide an answer. That is why it is important to have a strong title, and to clearly ask what you are looking for.

## Do you ask smart questions?

Being experienced in trying to learn how to solve problems on my own, by which I mean using the internet to search for the answers, I am already fairly comfortable with asking smart questions. I know that what I search needs to clearly state what I am looking for. While I have yet to post my own question on a website like Stack Overflow, searching through to see which questions got answers, and which ones did not made it clear to me how important it is to ask smart questions.
