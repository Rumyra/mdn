# Owners Handbook

This provides owner guidelines for the MDN organization. Owners are those that work on the core team at Mozilla and manage community requests, access to repositories, content proposals and platform updates.

## Contents

- [Platform updates](#platform-updates)
- [Managing peers]()
- [Translated content](#translated-content)

## Platform updates

Or new features. These will usually come in the form of issues raised on other repositories, or issues raised within the dedicated project itself. New issues for platform updates should have the `Engineering request` label added.

Time is set aside every fortnight (vaguely a sprint) to work on platform improvements. They can be anything from new requests of features, to updates that would be helpful, to urgent issues that affect our users.

Issues should be read and discussed. If there are any irrelevant issues, they should be closed with the `wont fix` label applied, and a comment explaining why. `on hold` should be applied if there are any blockers to doing the work. If the issue has been added to the project by mistake and should exist elsewhere, move it.

An issue should be reviewed with the following criteria:

- Priority:
   - `p0` Urgent: Something is broken and needs to be fixed immediately.
   - `p1` High priority: This is needed, but not something that's broken and affecting our users.
   - `p2` Medium priority: It would be great to get this done if there aren't any other high priority tasks, chances are this issue will escalate to high priority soon enough.
   - `p3` Low priority: This is a nice to have. Small chance of it escalating, but something we should consider.

- Time:
   - `time: -30mins` Less than 30 mins: A quick fix, a ten minute task, however no task is just ten minutes but the developer can change, test and pr within less than an hour.
   - `time: -3hours` Less that 3 hours: This change will take about half a day for a developer to modify and test and raise a pr.
   - `time: -2days` This task will keep an engineer involved for a day or two. Or more than one input is needed, such as a fix from front end as well as back end.
   - `time: multi day` This task will take a few days or more to complete. With these type of issues there are probably sub-issues which should be raised, or more definition needed. Multiple engineers are probably needed (such as front end work and back end work).

This will give a good idea of what issues need and can be worked on. Issues that can be completed within the fortnight should be assigned and moved to the 'To do' column.

## Managing peers

### Requests

Peer requests should come through the request process. They be able to prove github experience and provide a resonable reason to becoming a peer. Ideally they will have provided an area or two of expertise (such as HTML or JavaScript).

It's your judgement call as to whether we add them as a peer. It's worth noting they will gain write access to our repositories so if you want to push back then please do. If you're unsure it's worth asking them to contribute more and consistently, which should give a better idea of what to expect from them.

If you're happy to add someone as a peer, make sure they agree to the issue triage process and pull request etiquette and code of conduct. Once that has happened you can add them as a member to the mdn github org. Add them to any appropriate teams so they can contribute to pull request reviews.

## Teams

Teams should be used to grant access to relevant repositories as well as assigning pull requests to relevant peers. Teams should be favoured over individual write access, as it's easier to see who has access to what.

Each team should have a minimum of three members and ideally two maintainers (those who have the ability to manage members). Invites can go awry so make sure the invited user visits either https://github.com/orgs/mdn/invitation or https://github.com/mdn/content/invitations

Here is a list of the mdn org teams:

### Core

**Core** This is the core mdn team. It's for those that work on the MDN team at Mozilla only.

**owd** This a team with members from OWD so we can allow access to private projects we work on at MDN

There is also a private Mozilla maintenance team which should not be removed.

### Content

**yari-content** This is the main team for all the sub content teams listed below. No one should be a member of this team directly but rather one of the sub teams.

**yari-content-mdn** This is the 'default' team. It contains people on the Content Team at MDN and core peers. It allows access to example & demo repositories (such as mdn/interactive-examples) as well as mdn/translated-content and acts as the default pull request review team for docs within content that don't fall into other categories below. Add users with caution as this allows quite a bit of write access.

**yari-content-accessibility** Accessibility Content team for reviewing pull requests associated with accessibility.

**yari-content-html** HTML Content team for reviewing pull requests associated with HTML.

**yari-content-svg** SVG Content team for reviewing pull requests associated with SVG.

**yari-content-css** CSS Content team for reviewing pull requests associated with CSS.

**yari-content-js** JS Content team for reviewing pull requests associated with JS.

**yari-content-http** HTTP Content team for reviewing pull requests associated with server side things.

**yari-content-web-api** WebAPI Content team for reviewing pull requests associated with Web APIs.

**yari-content-moz-add-ons** Web Extensions Content team for reviewing pull requests associated with Web Extensions.

### Content Pull Requests Reviews

Pull requests reviews on mdn/content and it's associative repositories (translated-content, interactive-examples et al) are assigned via the 'round robin' style of auto assignment. A team is allocated to a repository or area and the members are allocated pr reviews one at a time.

You can change and update who receives these review requests within each team via the teams settings.

You can change and update which teams are assigned to repos via each repositories respective CODEOWNERS file, found in the .github directory.


## Translated content

Requests for Translated content can either be support from the unfrozen locale teams or a team looking to unfreeze a locale.

### Support

The current locale teams are fairly self sufficient and requests from them are low traffic. Most can be dealt with by the guidelines set above as they will be platform updates or new features, or requests for peers to be added removed.

Anything else can be discussed directly with the contributor. If input is needed from a wider set of translated content contributors, open a discussion or issue on the [Translated content repository](https://github.com/mdn/translated-content) following the [issue guidelines]()

### Unfreezing a locale

The guidelines for a community member to request a [locale to be unfrozen are here](https://github.com/mdn/translated-content/blob/main/PEERS_GUIDELINES.md#activating-a-locale). They will get in touch with one of the core peers or owners through [appropriate channels](). If the request is agreed upon the locale can be unfrozen and added to mdn/translated-content.

Task list for unfreezing a locale

- Raise a platform request to unfreeze locale
- Communicate with requester time scale
- Create a team under the Translated Content team, with contributors, update the [CODEOWNERS file](https://github.com/mdn/translated-content/blob/main/.github/CODEOWNERS) and set team to be sent pr reviews for their locale prs
- Create a label on mdn/translated-content and mdn/content for that locale
- Update github action to move any issues on mdn/content with that label to mdn/translated-content
- Introduce requester to other locale teams - they will help with 'How tos' and other queries


