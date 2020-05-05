# Structure of deal.II documentation

3 levels of documentation

- tutorial
  - how deal.II is used in practice 
  - big picture, no detailed explaintation
  - the concepts of fem, building blocks
- manual
  - detailed documentation of every single class and function
  - microscopic view of things without information on how the fucntion fit into the big picture
  - not a good place to learn deal.II
  - **Main page** of the deal.II tutorial site
- modules
  - group of classes and functions that work together or have similar functionality
  - documentation at intermediate level, overview of what's there in a particular area
  - **Modules** tab of the deal.II tutorial site.

# Structure of deal.II tutorial

- intro
  - what the program does
  - math model
  - programming tech
- commented program
  - documented listing of source code
- results
  - output with comments and interpretation
  - suggestion for extension/ exercise
- plain program
  - source code stripped of all comments


# run the tutorial

    // decription of file dependencies & set up for compilation
    cmake .
    // compile all the soucres into an executable
    make
    // run the executable
    make run
# General suggestions

- think about documenting the code
- come up with ways to test the min-program
- Software carpentry for:
  - version control
  - make files
  - testing
  - Article: Best practice for scientific computing
- debugger: lecture 25
# step-1

## what this program does

two techniques
- syntax for generating triangulation objects
- elements of simple loops over all cells

three concept of fem
- an object of type **Triangulation** for the mesh
- call the **GridGenerator** functions to generate mesh
- **Iterator** to loop over all cells and iterators on mesh mesh-like containers


Plain code of step-1

    

    int main()
    {
        first_grid();
        second_grid();
    }