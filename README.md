# Amazon Tables Challenge

Uh oh, somebody dropped Amazon's database! They've hired you to help recreate it! We're going to use ActiveRecord and Rake to setup migrations and create new tables in our database.

## Instructions

First, let's create a `books` table with the following columns:

+ title
+ author
+ price
+ genre

Remember to run `rake db:create_migration NAME=create_books` to create your migration file. Inside of the migration file, define an up and down method like this: 

```ruby

def up
	create_table :books do |t|
		t.string :title
		t.string :author
		t.float :price
		t.string :genre
	end
end

def down
	drop_table :books
end
```

Once you've created your books table, create as many other tables as you can. Amazon needs a lot of different tables - look [here](http://www.amazon.com/gp/site-directory/ref=nav_shopall_btn) for ideas!

<a href='https://learn.co/lessons/hs-amazon-tables-challenge' data-visibility='hidden'>View this lesson on Learn.co</a>
