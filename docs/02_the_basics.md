# 02 The Basics



Although there are no stupid questions, there may be times when one is hesitant to ask questions in situations where the people around seem to be in the know already. The function of this section is to solve your shyness. In this section we try to explain the fundamentals of electronic publishing in order to help the reader formulate questions more precisely.


## What is a text?

A text is a collection of words and words are compositions of letters. In order to read a text we have all kinds of layout helpers. Keep in mind that in the Roman times (when texts were cut in stone) there was continuing writing: no spaces between the words. This was not considered a problem as reading was a craft only a few people mastered. These people knew the words and hence were able to read aloud, just try: *Icanreadthiseasilyaloud*. In time, the craft of reading became a common good and many design/lay-out helpers were introduced, for example spaces between words, capitals at the beginning of new sentences, commas, semicolons, colons and line breaks. Furthermore,  the notions of paragraphs,chapters and the like, developed into a standardized system that allowed for a smooth transmission between the structure the authors endowed their text with and the readers who became familiar to these standards. Thus enabling ease of reading and the possibility to read silently.

This structure of stratifying words into sentences, sentences into paragraphs and so on, including reading aids such as exclamation marks, bold and underscored text is called **markup**. It goes without saying that all these **markup** elements demand stable definitions and clear relationships. Everybody is free to invent their own rules (e.g., every first letter of a new chapter is a well-decorated small picture). For example, in the time of handwritten manuscripts many “free style” inventions were made. Some of them remained in our time and became part of the expended alphabet. Think of the ampersand “&”, it originated from the conflation of the letter e and the letter t – we call this conflations, *ligatures*. To define what we allow and what not, **Markup languages** emerged.

Markup languages are grammars that define the markup and the relations between markup elements. With the emergence of computer networks and the increasing need to standardize texts for multiple usages, an international ISO standard established in 1982 is called: Standardised General Markup Language (SGML). This logically structured markup language was a big step forward as it made a fundamental split between the text structure as such and the final representation of that structure. For example, contrary to languages used in word processors such as Tex, LaTeX, Word, Microsoft Word, Wordperfect or ODF (open office document format), where presentation and text structuring are mixed, SGML only defines functions or roles. When we type a **bold** word in the text using a word processor we in fact type “start bold” -\> type the word -\> “end bold”. <!--Kimmy and Loes, perhaps this can be made clearer with an image? -->
![your caption here](../images/_in_progress/03_1_intro_mixture_layout "MIXTURE")  
What is happening here is a mixture of **layout** and structure. Layout is the activity of presenting a text onto a medium, such as a paper page. SGML and its derivatives, the easier HTML (HyperText Markup Language) and the expanded XML (Extensible Markup Language) make a strict distinction between structure and
representation. A markup language knows notions such as “highlighted word or phrase” and then type 1,2,3... This allows you to equate e.g.: chapter heading with type1 and quotation with type 4. Depending on the output substrate you can then define in the layout phase how this will look like. For instance, a chapter heading is in a certain type font and font size and centred on the page, whilst a quotation is represented in the same font size and font of the running text, but now in italics. On a screen we can have things like chapter headings in pink and quotations in yellow. This freedom in the layout is explicated in a so-called **style sheet**, which is a table that connects a layout schema with the
markup schema. This way of working is imperative if one wants to allow a source text to be represented in many different ways on various media of various sizes. Note, that in many programs these translations are done fairly invisibly to the user. If we translate an .odt file into a .docx file,  all coding is translated one-to-one . As we will see in the following, translation between one file type into another is not always symmetrical. Hence, the golden rule is to **always make sure that the source text is as systemically structured as possible**.

An important notion is that all digital texts and accompanying coding are written in simple letters and numerals, this is called **flat text**. This is a stripped down text without layout; the most elementary token. It goes without saying that the flexibility of this process is limited to the character set for flat text we use. In the “old” days this was **ASCII** based and limited to the possible number of distinct signs (letters, numerals, commas, etc.) of a binary computer
text. Slowly but surely, a new list of allowed signs is making inroads. These sings are called: **Unicode**. Unicode aims to include all alphabets and letter systems including common signs and ligatures, such as the aforementioned & and diacritic signs. Again, this is a step forward to guarantee a clean source file for all kind of usages, even those we don’t consider or even imaging today.

### What is an electronic text?

An electronic text is normally understood as a text which is represented on a screen of some sort. Of course this is sloppy language. The key issue is that an electronic text became a structured file in which the emotions and intentions of the author are translated into notions like highlighted text of a certain type through the work of said author. Due to this markup, we become able to make different layouts, expressions, onto different media.<!--Pia: Joost kun je het voorgaande misschien iets specificeren? de link tussen de author en markup is mij nu niet duidelijk-->  It is of great importance to note  that electronic publishing introduces a big shift away from the page centred culture of book printing. Book printing allows for various  printing sizes depending on the wishes of the author, designer and publisher. For example, when making an art book based on a collection of paintings or drawings, a decission can me made on what the ideal book size is and whether or not it will be printed in oblong form or not. In the world of screens these types of decisicions are different as we have very different sizes of screens. No screen can be cut to the demanded size like with paper book publishing. In electronic books we have to work around things in a completely different way to the paper world. This means that the transposition from an existing work to an electronic representation is rife with difficulties if the structure of the texts and, in particular when the relation between illustrations and running text, is important. In the world of text based publications there normally 
only is running text. For these publications the page size is less important and this is part of the reason why e-readers are becoming
increasingly popular. On electronic reading devices the text can always be made to fit the size of the device, this is called **reflowable** text. In all other cases, the creator (publisher, designer, etc.)
has to consider how to design the work and under what conditions content and meaning are represented. This will be discussed in the following chapters for various outlets, as one might opt for various versions of the original work. It goes without saying that in the coming years, authors and designers will try and develop digitally conceived works that intrinsically allow for a variety of representations depending on the reading device whether electronic or not. 

### What is an electronic publication
<!-- Silvio: I'd maybe add a subchapter titled "what is an electronic publication?" in which i'd express the fact that ebooks are not necessarily in conventional forms such as epub or ibook, mentioning for instance project gutenberg where the majority of ebooks are general-purpose txt files. I would do so in order to explain that a structured text file pave the way for new formats of publication that involve non conventional publishing platforms like email, twitter, etc. --> <<!-- Pia: I think this section then gets too much weight, so I would leave it as is -->

## Electronic possibilities

Novel electronic capabilities enable a great number of possible
publication outlets. Before entering into the problematic aspects of
such a plurality of presentations of the same message, we investigate
the possibilities. As with all technological possibilities; the coin has
two sides (leaving aside the unstable rim) which exclude each other. The
printing press introduced pagination and indexing, allowing many
thousands of identical texts to be read and compared by an expanding group of readers over the years, independently of location. In an electronic
world with non-fixed screen sizes this is complicated. On
paper text is fixed, this allows for comparisons and interactions
between different readers separated in space and time. In an
electronic version the fixity of the text remains, as the text file is
independent from its final substrate (E-ink, lcd, paper), but its
presentation on to the final substrate can vary substantially. Think
about the introduction of numbering phrases in the Bible, which came
along during a ceremony when the priest wanted everybody in the
audience to read at once, however as the formats of the Bibles were non
standardised, page numbers were of no help. <!-- is there more information to back this anecdote? e.g name of priest, year this happened? -->

The challenge becomes even greater if we widen our ambition to pictures,
audio and video, hyperlinks, etc. In the Toolkit project, we deal with the field of books in the arts. This category of books integrates all aspects of text-only publications but
expands it with visual information that can be explanatory of the text
and, more importantly, to visual information which can be a 'stand
alone' statement. In such cases, text, helps the 'reader' (viewer) to have an understanding of and have a deeper appreciation for the object. It is clear that various forms of art books demand and enable different electronic
representations. In these books we witness a crossover between the
primary importance of text and image.

As cultural standardization over the centuries rendered, for example, a detective, religious or an educational book instantly distinguishable by its typography and layout, - this too willalso become a fact for electronic books. Apart from the electronic (or
paper) book as a 'object d'art', electronic art book publishing will
have many commonalities despite its difference in genre. A major issue
is that the electronic sub-structure makes all files just bitstreams
(streams of binary code: zeros and ones). The digital files containing
the various kinds of information are all equal on this level of digital
bitstreams in the computer memory: merely standardized code. The great
new thing in the world of electronic art books is that based on
standardized, though well tailored structures, the creative message can
be published in a great variety of ways. This not only depends on the
capabilities of the output (reading/viewing/listening) device, but also
on the function of the book for the author, in a present context, such
as a dictionary, a study, a reference, a coffee table book, or a leisure
book. The same source can and will be represented differently under
different circumstances. All these vistas demand a thorough and more labour-intensive editorial and production strategy. Not only because the same source can express itself in various output forms but even more so because once properly edited and stored electronically, information and its constituting parts can be reused and used in different ways, to be decided upon given a specific environment of goal, now and in the future.

<!-- Silvio: Here I'd maybe add that these possibilities require more work for all the parties involved. An example comes from web design: since the advent of responsiveness the work of designers doubled. -->