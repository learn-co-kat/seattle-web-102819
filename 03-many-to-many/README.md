# One to Many Relationships

## Questions??????
-

## TODO Lecture Outline
  - One-to-Many.
  - Introducing our Assessment for the afternoon

## SWBATs
* [ ] Implement one object to many objects relationship
  * [ ] One object `has many` objects
  * [ ] One object `belongs to` another object
* [ ] Practice passing custom objects as arguments to methods
* [ ] Demonstrate single source of truth
* [ ] Infer type of method (class or instance) through naming conventions
* [ ] Model/Domain
* [ ] Practice keeping groups of data related to classes on the class as a class variable
* [ ] Demonstrate _Single Source of Truth_ by **not** storing collections of objects on other objects
* [ ] Demonstrate _Single Source of Truth_ by **not** storing one object in multiple collections

## Deliverables
* **Create an Author class**. The class should have these methods:
  * [ ] `initialize` which takes a name and age
  * [ ] `name` that will a string
  * [ ] `age` that will return and integer
  * [ ] An author's `name` cannot be changed but their `age` can be updated
  * [ ] `books` that returns an array of Book Instances that this author has written
  * [ ] `write_book` that takes a title, creates a new book, and adds it to the author's book collection
  * [ ] `books` a books array to keep track of all the books the author has written.
  * [ ] `book_count` that return all the books this author has written
  * [ ] `top_author` that will return the author and book count of the author with the most books written
* **Create a Book class**. The class should have these methods:
  * [ ] Have a mini breakout and see which methods would be instance vs class.
  * [ ] Book has a method `#title` that returns a string.
    - this is a getter method
  * [ ] Book has a method `#author` that returns an instance of the author
    (1st answer)
    - class method -> because books only belongs to one author.
    - instance method -> getter.
  * [ ] Book has a method `.all` that returns all the Books created
  * [ ] Book has a method `#author_name` that returns the name of the book's author

## Outline
* Relationships (one to many => `has_many`, `belongs_to`)
  * Go through other example domains
* Expand on relationships to express many to many
  * We'll build out a **new** relationship from scratch to teach this concept

## Define
* _Model_ - A class whose primary responsibility is to store data
* _Domain_ - The subject matter of the problem, (e.g., Learn's domain is online education)
* _Domain modeling_ - Creating models for your domain to represent real or abstract ideas (e.g., Learn's domain model includes modules, cohorts, assignments as well as their relationships)
* _Relationships_ - How one model or thing is connected to another model or thing
  * _One to many relationship_ - A relationship describing a single model that contains or keeps track of other models (a tree has many leaves, an organism has many cells, the universe has many galaxies)
* _Schema_ - A visual representation of your data (models, relationships, etc.)
* [_Single Source of Truth_](https://en.wikipedia.org/wiki/Single_source_of_truth) - The practice of structuring _models_ and _relationships_ such that every data element is stored exactly once; any possible linkages to this data element are by reference only
  * **Why?** - Ask yourself, in the _one to many relationship_ of country to citizen, is it easier for the country to know about all of its citizens or is it easier for a citizen to know the which country they belong to? So how does a country find out its citizens? It conducts a census (a method) that asks all the people in the country if they are a citizen!
