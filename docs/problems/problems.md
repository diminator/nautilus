# Problems

## Problems

1. Solving problems through `problems` is slow at the start of a project when many decisions must be made and many factors considered (on the flip side, decisions can be taken carefully with every relevant factor considered explicitly)
2. A decentralized web of forks imposes difficulty on new contributers by introducing difficult-to-answer questions:
   - Where is the most up-to-date source of truth?
   - If a new piece of knowledge resides in one repository, could its surrounding context be out of date?
   - If I create a new piece of knowledge, where do I share (pull request) it to?
   - More generally: what is the difference between different forks at any point in time (might require knowing more about each fork maintainer)?
3. Using Github imposes a penalty on potential contributors who are not familiar with:
   - The command line
   - The git command
   - The Github web interface
   - Decentralized git workflows
4. `Problems` stored in the `/problems` folder have no state, which means you can't tell from the outside:
   - When a problem was posted
   - When a problem was last updated (actually you can see this from the commit record, but is it good enough?)
   - Whether it's been solved
   - If it hasn't be solved, what the status is: who's working on it, which solutions are being considered, when it's expected to be resolved.
5. Don't know how to relate a proposed or adopted solution to a problem (related to #4)

## Solutions

### Per-Item

1. (No proposed solution.)
2. See 'Centralize'
3.
   - Provide educational courses for everyone involved on a regular basis
   - Create a public Google Drive folder that can be cross-referenced by this system
4.
   - Use Issues instead
     - Problem: can't be easily merged into new repositories
   - Include meta-data at the top of each file
   - Put the filing date in the filename
   - Put the status in the filename
5. Give each problem a UID by which it can be referenced in the same file and elsewhere

### Centralize

- Centralize Nautilus under an Ocean account / org and (at least) nominate this the official upstream fork
- Nominate diminator/nautilus as the de facto upstream repo and document it
- Maintain a list of all possible upstream repositories to keep in sync, maintain a manifest explaining the purpose of every branch, and document a decentralized workflow (works for repositories, but not for issues)
  - http://52.59.198.28:8080/ (?)
- Use a collaborative document editor with a single source of truth (like Google Docs)

## See Also

- https://github.com/TimDaub/nautilus/issues/2