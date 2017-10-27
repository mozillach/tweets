# @mozillaCH Content Queue
## The concept
This repository serves as a curation tool for the [@MozillaCH](https://twitter.com/mozillaCH) Twitter account. Each issue represents a Tweet or Retweet on that account. The issue gets validated by a service, if it is tweetable. If it is deemed ready and the curators of the Twitter account accept the content it will eventually be tweeted. This allows any user with a GitHub account to suggest content for the Twitter account while still retaining control over what is actually tweeted. Further it simplifies letting multiple users tweet from a single account.

## How to submit a tweet
### Open an issue
To suggest tweet content, open an issue in this repository and fill out the issue template. The issue will be added to the "Ideas" column on our project board.

Tweets should be English, though linked content does not need to be English. You can attach images by uploading them to the issue and embedding them using the GitHub image syntax in the tweet content.

#### Scheduling
A tweet does not need to be scheduled to a specific time. Please only schedule it to a specific time if the content is time-sensitive, like event notices or campaigns. To schedule a tweet, add a `## Scheduled for` section with a date in the format of `DD.MM.YYYY HH:mm`. The time stamps are interpreted as UTC+1. Example:
 ```md
 ## Scheduled for
15.11.2017 18:00
 ```

#### Replying
To reply to a tweet add a `## Reply to` section to the issues and paste the link to the tweet to reply to as its content. Example:
```md
## Reply to
https://twitter.com/MozillaCH/status/917786667259482124
```

#### Retweeting
The template suggests a normal tweet by default, but you can also retweet a tweet by changing the `## Tweet Content` heading to `## Retweet` and pasting a link to the tweet to retweet as its contents. Example:
```md
## Retweet
https://twitter.com/MozillaCH/status/917786667259482124
```

### Ensure content is ready
The service will assign the "ready" label, once your tweet satisfies the formating restrictions of the service and its contents will be tweetable. It will report any outstanding issues else.

### Getting tweeted
Curators will now take over and first move the issue into the "Proofread" column and someone will be assigned to proof read it. Once that is done and potential spelling mistakes are fixed, the issue will finally be moved to "To Tweet" where it will be tweeted.

## Automated tweet sources
### Mentions
Mentions are automatically added to the "Needs Reaction" column and a curator is assigned to handle creation of a reply. It then moves through the same stages as a tweet submitted as idea.

### Reps events
Events for the filter query "switzerland" (the same query used for the events widget on mozilla.ch) will automatically be added to the "Events" column. It has its due date set for the event start. Curators should then at least create an announcement tweet from it and move it through the same stages as a tweet submitted as idea. Optionally a retweet of the tweet should be queued once the original event tweet was tweeted.

## Contribution guidelines
If tweet content is changed last-minute after the tweet is approved for reasons that weren't discussed in the issue, we may exclude you in the future from submitting tweets.

The general [Mozilla Community Participation Guidelines](https://www.mozilla.org/en-US/about/governance/policies/participation/) apply.

## Curators
Curators are members of the mozilla.ch community that are active around the mozilla.ch Twitter account and moderate tweet content in this repository.

### Becoming a curator
After 5 of your tweets have been successfully approved, you can nominate yourself as a curator by opening a thread in our [discourse category](https://discourse.mozilla.org/c/communities/switzerland). Please also mention if you intend to handle mentions to the Twitter account or not. At least two curators who have interacted with the nominee in the context of this repository before must vouch for them for the nomination to pass.

Members of the [focus group](https://wiki.mozilla.org/CH#Focus_Group) can get curator status without formal self-nomination.

### Staying a curator
Curators who have not interacted with the repository for 3 months may have their access rights revoked, but can re-nominate themselves at any point.

### Being a curator
Curators should not move issues with tweet content they created through the board. Curators should self-assign themselves to an issue if they are handling its movements through a board and are coaching the contributor that is authoring a tweet.

#### Mentions
Curators can volunteer to also handle mentions, where they will be assigned in revolving order to incoming mentions on the Twitter account and will author replies. A curator may defer to other community memebers to suggest content for the reply, but only curators will be able to actually author the tweet (since the issue created by the service has to be edited).

#### Proof reading
Curators that feel confident in English orthography and grammar should proof-read tweets pending in the "Proofread" column and move them to the "To Tweet" column when tweet content is error-free and they have not authored the content themselves.
