# Quote DB

I've collected quotes over the years, and they are scattered in many places, many formats, and many styles. This is an attempt to put them all in one place and keep them there.

## Quote Keys

In some for or another, the following "keys" have been used to hold quotes:

- cite
- text
- node
- title
- note
- keywords
- source
- img

## rails new command

    rails new quotedb -d postgresql

`.railsrc`:

    --skip-spring --skip-turbolinks --skip-action-cable --skip-sprockets --skip-listen --skip-coffee --skip-test --skip-system-test --webpack=react

### update Tue May 21 12:18:36 2019

Turns out, to use the `GraphiQL` front end to the GraphQL server, you need sprockets! Uncommented it in the `config/applicaton.rb` file.

## Initial Structure

- Quote model
- Keyword model (might call this Tag instead)
- Taggings - a join model between Keyword and Quote (better than KeywordQuote as the default for join models in Rails)

## Thoughts on Front End

I've been developing using the `webpacker` and `react-rails` gems, which provides the `react_component` method. In this app, I'm going to try to just use the `webpacker` gem alone, though still implementing react, but not use the `react_component`, just use the packs to create the client. We'll see.

## GraphQL or not?

I've also been using GraphQL a lot, I'll probably use it here, simply because I like it a lot. For the front end, I'll add in Apollo Client as well.
