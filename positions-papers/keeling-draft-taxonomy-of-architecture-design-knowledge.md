# A Drafty Taxonomy of Architecture Design Knowledge

Like many journeys, packing starts with a list.  What are all the _things_ a
software architect needs to know to be able to...

* Understand a problem and divine stakeholders' concerns?
* Explore potential solutions?
* Evaluate options and make decisions?
* Make concrete representations of the problems and solutions to aid in
  communication, understanding, exploration, and evaluation?
* Evaluating how well the design manifests in the living breathing system?
* Organize the team (however large or small) around stakeholders' concerns to
  design the architecture, create it, and evolve it over time?

Within minutes my list enumerated over 50 items.  Many items were hand-wavy nods
to _insert more things here that are under this category_.  The Architecture
Island instructions were clear:

> Unfortunately, due to cargo restrictions, it is not
> possible for you to bring all the architecture, design, and
> programming books from your personal library.  There is only
> enough room for the most important information.

I need to make some serious cuts, but my list was overwhelmingly long,
unwieldy.  I had a list of _things_, but items on the list were dramatically
different, almost incomparable.  I had methods.  I had concepts.  I had
fundamental ideas.  Processes.  Artifacts.  Tasks to perform.  It was a great
list.  A great list that I couldn't possibly cull.

"I know," I thought to myself, "I'll add some categories!"  That way
I'll be able to pick and choose from across categories, ensuring I've selected
a representative set of knowledge.

Initially the categories were helpful but soon they too became an unwieldy mess.
Some items on my list belonged to multiple categories.  What's more, the
categories themselves represent _bits of knowledge_ that need to be packed!

Next idea.  Maybe if I organize the categories into a rough hierarchy, I'll 
stand a chance of tagging all the ideas in the list?

Here is the (incomplete) draft result:

<object data="https://github.com/michaelkeeling/saturn2019-architecture-island-workshop/raw/master/positions-papers/keeling-architecture-knowledge-taxonomy.pdf" type="application/pdf" width="700px" height="700px">
    <embed src="https://github.com/michaelkeeling/saturn2019-architecture-island-workshop/raw/master/positions-papers/keeling-architecture-knowledge-taxonomy.pdf">
        <p>This browser does not support PDFs. Please download the PDF to view it: <a href="https://github.com/michaelkeeling/saturn2019-architecture-island-workshop/blob/master/positions-papers/keeling-architecture-knowledge-taxonomy.pdf">Download PDF</a>.</p>
    </embed>
</object>

## What's in the taxonomy?

The root of the taxonomy is software, or perhaps more specifically
_software-intensive systems_, since there is more to building software than
only the code.

At the next level, the node that we care most about is architecture.  It helps
to add siblings at this level, which are other software engineering
disciplines.  Some examples might include project management, quality assurance,
and configuration management.

The next level shows broad categories of the types of things architects will
need to know.  I currently have this divided into three big buckets, but I'm
not convinced it's 100% correct.

The next levels help classify information within these broader buckets,
eventually getting down to specific patterns, structures, methods, and
approaches.

The bottom-most level is largely contextual, mean to show that there are 
specific instantiations of these ideas that can vary from team to team or system
to system.

Given the number of levels it seemed prudent to assign a name to each level. I
chose to use the taxonomic ranking from biology simply because I was familiar
with it and it approximately corresponded to nodes within the taxonomy.

## How might use such a taxonomy?

Organizing knowledge is helpful for prioritizing.  As a start, it gives us a way
to designate some knowledge as being clearly "in" or "out" of scope.  For
example, we may choose to say that the idea of patterns are useful but choose
not to exhaustively enumerate all patterns, or perhaps choose only to focus on
_Families_ of patterns, leaving the _Genus_ as an exercise for architect.

We can use the taxonomy to ensure we have selected representative knowledge.
Are we lopsided in one area or another?  Do have an appropriate breadth of
information?

Finally, the taxonomy can also help us prioritize within a category.  For example
if we decide that lean documentation methods are important, then perhaps we
can focus on selecting a _top 3_ representative examples.  This way we avoid
comparing apples to oranges or picking between things that are ultimately not
comparable.

## Weaknesses in the taxonomy

The draft is just that -- a draft based on a few hours of thinking.  Keep this
in mind when considering the specific nodes.  Ultimately I found the taxonomy
to be more interesting than the list I used to discover it, so the bottom parts
of the tree are much less detailed.

Finally, there may be some areas of the tree that overlap.  I'm not sure if this
should be allowed or not.  In biology we generally want strict separation.
That said, there still exists an occasional zoological oddity.  The platypus is
an [egg-laying, duck-billed, beaver-tailed, otter-footed,
venomous mammal](https://en.wikipedia.org/wiki/Platypus), which defies many conventions
established for mammals.  As we get to lower levels of the taxonomy, the possibly
of overlaps increases, which implies there are problems in the taxonomy, or perhaps
the premise itself.
