# How to write good commit messages

#### The seven rules of a great Git commit message

  * Separate subject from body with a blank line
  * Limit the subject line to 50 characters
  * Capitalize the subject line
  * Do not end the subject line with a period
  * Use the imperative mood in the subject line
  * Wrap the body at 72 characters[^1]
  * Use the body to explain what and why vs. how

!!! note "Your subject should start with one of the following"
    * feat: The new feature you're adding to a particular application
    * fix: A bug fix
    * style: Feature and updates related to styling
    * refactor: Refactoring a specific section of the codebase
    * test: Everything related to testing
    * docs: Everything related to documentation
    * chore: Regular code maintenance.[ You can also use emojis to represent commit types]

#### Template

    Capitalized, short (50 chars or less) summary

    More detailed explanatory text, if necessary.  Wrap it to about 72
    characters or so.  In some contexts, the first line is treated as the
    subject of an email and the rest of the text as the body.  The blank
    line separating the summary from the body is critical (unless you omit
    the body entirely); tools like rebase can get confused if you run the
    two together.

    Write your commit message in the imperative: "Fix bug" and not "Fixed bug"
    or "Fixes bug."  This convention matches up with commit messages generated
    by commands like git merge and git revert.

    Further paragraphs come after blank lines.

    - Bullet points are okay, too

    - Typically a hyphen or asterisk is used for the bullet, followed by a
      single space, with blank lines in between, but conventions vary here

    - Use a hanging indent

    If you use an issue tracker, add a reference(s) to them at the bottom,
    like so:

    Resolves: #123

#### Example

    Re-enable React server-side rendering
    
    Move render string output directly into template creation portion of the 
    template render call.
    
    By moving the render string out of Koa state, we no longer have memory 
    allocation issues:

    Results: https://cl.ly/abcdef123456

    Resolves: #123

[^1]: Each line in description should be limited to 72 charectars

!!! note ""
    Use ```git commit``` instead of ```git commit -m``` as the first command opens a editor in cmd and the later expects to be entered the message in the same line.

    