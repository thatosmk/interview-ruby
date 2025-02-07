## About The Project

This repository is meant to act as a skelleton for you to develop a simple ruby application that serves a singular purpose as outlined below. You are required to work with ruby 3.2.3, but you can add any Gems you like in the Gemfile to serve your purpose. We recommend using rbenv or rvm to install one if you currently don't have any.


## Getting Started
Install [RVM](https://rvm.io/rvm/install) or [rbenv](https://github.com/rbenv/rbenv) and use it to install ruby 3.2.3

Install bundler with `gem install bundler -v 2.4.19`

Run `bundle install` to run Bundler

Ruby `ruby process.rb --sample` to run the basic case. It should output 'it works' on console.


## Introduction

Analyse the PDF Given in `files/ast_sci_data_tables_sample.pdf`. Data extracted from the two pages in the PDF are in `pages/1.json` and `pages/2.json`. The data is
arranged in Arrays of hashes with the following key attributes:

  * BlockType: Can be one of `PAGE`, `TABLE`, `LINE`, `WORD`, `TABLE_TITLE` and a bunch of others
  * Id: Distinct ID per block
  * Text: For the type `WORD`, this field contains the text extracted
  * CellLocation: For the type `CELL`, this contains the location of the cell
  * Children: Array of Ids of blocks that are directly descendent of the current Block
  * Geometry: Location of the text extracted from the PDF

There are some attributes that we'd ignore for the purposes of this excersize.


## Task

The purpose is to extract the contents of all the `TABLE`s of all the `PAGE`s and print them out as given in 'solution.png'

## What we look for

This is an excercise to determine how well you can understand a problem and structure a solution. The final result is not the only thing we're after, make use of all the Ruby you know and all that Ruby has to offer.

Also keep in mind that this is a simpler representation of a real world problem, so we'd consider everything from memory, performance, code structure, cleanliness, commenting etc. Imagine this code to be a part of a much larger project worked on closely by a team of 10 developers.

We would like to know how long did it take you to finish the problem from reading this file to getting the output.

Best of luck.



