# Hunter
The only legacy we can leave behind for our juniors.

## Goal
A website which makes them aware of various opportunities at the right time so that they never miss them in unawareness.

### Overview
-[] write python script for scraping all relevant positions(indian and remote only leaving other to keep the noise to minimum) from various careers page of all the companies listed in morethanFAANGM repository.
-[] same for all opensource contribution programs and try to fetch the dates and update if date is coming soon.
-[] same for all internships, apprenticeships, fellowships, scholarships or any other kind of ship... (scrape social media platforms for these terms)
-[] scrape for gh-bounties through search query in gh using issues tagged with bounty.
-[] (little distant future) provide user login facilities for customising alert of their choices.

### Infrastructure
Everything is decided in such a way (atleast till now), so that nothing apart from github is needed to deploy such a project can be kept running with least or no maintenance requirements.
For example, python scripts can be ran using github actions once in a day and data generated can be stored in .json files with a predecided structure so that website can keep displaying all the various opportunities without any need to maintain database or backend.
For things like scraped results from social media, human intervention might be required to verify if the particular post is relevant or not. This can be handled by creating issues for each post grabbed through social media for human verification and then can be closed if not relevant. Using Github Api, all of the open issues will be obtained and displayed on the website.
Many projects seem to incentivize open source development and offer bounties on issue-by-issue basis. Such issues can be found using github.com/q?= with label for bounty.
Since issues have template feature, one specialised label something like 'sign-up' can be created where user will have to put details in the issue template as mentioned there.(This sounds inconvenient but the people interested in Hunter will always, atleast most of them, have a github account already.)
