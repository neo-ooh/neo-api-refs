# Glossary

### Undefined Behaviour – UB
When building the API, their is some edge case that doesn't make sense in the sense of API. (eg. Giving an email to a group). For ease of implementation, these actions are not prohibited, but their consequences are not tested, resulting in what's called an *Undefined Behaviour*.

Keep in mind, an Undefined Behaviour is something that is *known* and whose existence is documented, otherwise its a bug.