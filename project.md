# Project proposal

## The user and a language

This language is to digitally create quilting pantograph patterns that can be printed out and used on a long-arm quilting machine.

### What's the need?

_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help
them?_

This language is meant to help amateur home-quilters create and quilt more elaborate quilting patterns. Long-arm quilters currently have limited options for creating paper pantographs - if they want a digital pattern to print out, they can either buy a pattern for $15-25 online or buy quilting software to help automate this task. If they wish to create their own, the easiest way is to hand-replicate a pattern, or create one in an aformentioned quilting software and print it out.

Ideally, this experience could be made easier by having a dedicated platform to make pantographs that can create and modify the line design, as well as visualize how it gets repeated across a quilt surface, and being able to print it out according to quilt size specifications.

### Why a language?

_Why is a DSL appropriate for your user(s)? How does it address the need?_

I believe a DSL is appropriate for the need because it could leverage the automation of patterns, and quickly propogate an idea to visualize the larger pattern. Drawing one shape is probably easier by hand, but to have it be a pattern and then be the right size to print and then quilt is a more complicated procedure, that could benefit from all of those things being in the same place. In other words, since design aesthetics are a crucial component of this step in the quilting process, streamlining things like whether a design is a valid continuous line, with entrance and exit points at the same place, and being able to see how it would visually look across a quilt can help improve the creating and prototyping process of a pantograph design. 

As far as quilters using a programming language goes, computer aided design tools are often not compeletely unfamiliar to quilters and so I'm only marginally worried about a learning curve in terms of what a user might find uncomfortable to use, though it is something that I will keep in mind during the design process.

### Why you?

_What excites you about this idea? How did you come up with it?_

I like this idea because I'm a quilter myself, and it's been interesting to learn more about this technique and the technology available for it. Long-arm quilting is not something I personally do because I don't own a machine, but the quilting designs themselves are as important as the piecework of creating the quilt-top so I came up with it as I was exploring the patterns different textile artists create. I think it's exciting to potentially create a tool that will aid quilters in a part of the creation process that often gets outsourced, and offer them another degree of creative freedom.

### Domain

_Describe the project's domain in five words._

Digitizing quilting pantograph creation process

### Interface (syntax)

_How might the user interact with the language? What does programming look
like? Why is this the right way to interact with the problem domain?_

Ideally, I'd like the user to be able to interact with the language in a combined approach of settings/menus, and textual interaction. The continuous line design itself, as a singular object, would be created using a written language similarly to other written designing languges for simulation or visually creative designs. Then quick modular operations, like rotations, importing an existing design, flipping a design, and settings for the view window would be menu buttons. 

I think this is the best way to interact with the domain because it still allows for maximum control over the line design itself, while making easy overall design choices, and modifying ways to view the overall design, more intuitive especially for users who are likely less familiar with coding.

### Operation (semantics)

_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When the program runs, the user would be able to see the design in a window as a finished pantograph. They could then edit the view of the design by adding/viewing measurements, adding grid lines, changing whether it was a border design or edge-to-edge, what the final size of the quilt is and more. The types of errors that might occur that are important to the user are mostly aesthetic - if the shape didn't "pattern" the way they expected, or there were some parameters that were a bit strange, or they just decided they didn't actually care for the design. All those errors could easily be communicated through the design window and the artist can then decide what to do next. There could also be syntactic errors wouldn't compile, and it would ideally show the user where it went wrong. Communicating these errors clearly is probably going to take careful time, as well as communicating logical errors. Potentially, adding a way to highlight where a line design is not continuous, or doesn't have the same entrance/exit points could be very helpful to a user in troubleshooting the ways their code was affecting the design.

### Expressiveness

_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

The main function of this language is to visualize a pattern from a smaller design. So it should be really easy to create an image using only lines, most often just one continuous line, and then visualize that design either by itself, or repeated to make a larger design. It should then also be easy to export the design into a printable format that quilters can use. It will probably end up difficult to create patterns using data visualizations since I intend to also make it difficult to perform operations like calculations. I'm imagining something somewhat similar to ContextFreeArt in terms of what operations it can do, if not the actual purpose or implementation. In other words, I think if the code can then be translated into a line design it won't be completely impossible, but may still be difficult to stretch that scope. Inside scope, I would aim to make the code as streamlined as possible, interms of the language design, but also what of what operations gets abstracted away from the textual language.

### Related work

_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There are not really any other DSLs that I could find. There is a software called Electric Quilt 8 (EQ) https://electricquilt.com/online-shop/category/electric-quilt-8-eq8/ which is an interface for a digital quilting design process, including pantographs, but also including lots of other parts of the quilting process. From what I can tell, it's not a bad tool, but if you just want to create pantographs, it feels hard to justify a several hundred dollar license purchase. I do like that in EQ8's pantograph function, they have the ability to both create and import pantograph patterns. There is also a company that sells frames and quilting machines that also sells an automation software that has the ability to create pantographs https://graceframe.com/en. However, it is similarly expensive unless the quilter's goal is to create a more professional home setup.

## The Project

This section examines whether the idea makes for a good CS 111 project.

### Suitability

_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

### Scope

_How big an idea is this? How ambitious is this project?_

### Benefits and drawbacks

_Why might this be a good idea for a project? Why might this not be a good idea
project?_
