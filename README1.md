## How would you return all the recipes in your database?
Recipe.all

## How would you return all the comments in your database?
Comment.all

## How would you return the most recent recipe posted in your database?
Recipe.last

## How would you return all the comments of the most recent recipe in your database?
recent_recipe = Recipe.last
recent_recipe.comments

## How would you return the most recent comment of all your comments?
Comment.last

## How would you return the recipe associated with the most recent comment in your database?
recent_comment = Comment.last
recent_comment.recipe

## How would you return all comments that include the string brussels in them?
Comment.where('content LIKE ?', '%brussels%').all
