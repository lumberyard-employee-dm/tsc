# TSC Meeting -7/11/2023

## Chair and Co-Chair
* nick_l
* Tobias Alexander Franke [Huawei]

## Attendees
* Nick_L 
* geds-dm [Amazon]
* colinb [APMG]
* Nicholas [Red Hat]
* null [Amazon]
* Alex P [Amazon]
* Royal OBrian [LF]
* Naomiwash [LF]
* Sid_Moudgil [Amazon]
* Nicholas [Red Hat]


 ## Agenda Items
[https://github.com/o3de/tsc/issues/83](https://github.com/o3de/tsc/issues/86)

Two topics were discussed: 
* Content approval process for canonical.o3de.org remote repository
* Are we going to include Features Grid for the next release?

## Content approval process for canonical.o3de.org remote repository
The RFC is located at https://github.com/o3de/sig-content/issues/143

Alex P: discussed the RFC for the Content Approval Process of getting content into O3DE
Alex P: The goal is to add a lot more content to the canonical repo to see extra content to download as part of Project Manager
Alex P: Was wondering if LF Legal Approval is needed at the current time?
Royal OBrian: We should wait until if the RFC is something that we want to do first before contacting legal
Royal OBrian: Binary content would need to be uploaded to o3debinaries.org, Asset content can be sourced from the repo
Royal OBrian: Clarified that non-code content license for o3de is Creative Commons, with source code being MIT/Apache2
geds-dm: Should SIG-Content own the approval process? It seems unrelated to SIG-Content current responsiblities
Royal OBrian:

Colin B: Could some of the gems that are part of the o3de/o3de be moved out such as the AWS Gems
Alex P: Yes, that work is in-progress and will be part of another repo

The discussion transitioned over to the 3rd Party system
ColinB: Was having issues building 3rd Party libraries that are part of the 3p-package-source repo
Nick L: If there are build issues with a 3p package, that is a bug
Nick L: Linux foundation needs the keys to upload 3rdParty libraries
Nick L: Also the 3rd Party upload process should need to be automated to build in a safe Jenkins environment to prevent malicious tampering with the package before upload
Royal OBrian: We need the packages to be signed
Nick L: The packages are signed after every build, however they are built on the Developer machine and therefore aren't safe for tampering
Colin B: Development team rebuilds binaries or pin


## Feature Grid Updates
The agenda is linked https://github.com/o3de/tsc/issues/85#issue-1786957640
A question from from the 23.05 release retrospective of whether we should use the Feature State Form should continue 

There are claims that it takes hours to update the Feature State Form for release
Royal B: The markdown generated from the Feature State Form is just generated from a script in the community repo
Royal B: Can be contacted by the release team to figure what the HTML changes needed to be placed around the feature
Royal B shared screen to show that [Sample-FeatureMarkdowns.md](https://github.com/o3de/community/blob/main/features/Sample-FeatureMarkdown.md) is what would be generated by the feature state tool

geds-dm: The Feature Grid that is shown on docs.o3de.org is markdown as well
Royal B: Found that the 22.10 release markdown in the o3de/o3de.org repo is similar to the content that is in the Sample-FeaturesMarkdown.md
         That markdown file is located at https://github.com/o3de/o3de.org/blob/development/content/docs/release-notes/archive/22-10-0/feature-state.md
Royal B: The release markdown file for the o3de/o3de.org repo contains github specific markdown.
         Will investigate the similiarities between both markdown files.

# Emerging Topics

Naomiwash: Shared a document about the O3DE Community processes about the logistics of running a SIG (https://github.com/o3de/tsc/issues/86#issuecomment-1631092223)