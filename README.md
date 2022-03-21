# AccessMap Wiki Summary
AccessMap provides a customizable pedestrian navigation experience on web, Android, and iOS. Explore your city and get helpful routes that fit your mobility profile.

There are many apps and sites to help people navigate by car: Waze, HERE, Apple Maps, Google Maps; all these apps offer some semblance of 'pedestrian' directions, but make gross assumptions about what hills you can take, how speedy you will be, what is a 'safe' walking or rolling environment, and many don't even provide basic information about whether or not there's a sidewalk there. AccessMap, previously a web application produced by the [Taskar Center for Accessible Technology](https://tcat.cs.washington.edu/) is bringing mobility equity to pedestrians by improving and customizing walking/rolling routing.

For International Day acknowledging Persons with Disabilities (Dec 3 #IDPWD2021) the group is releasing the mobile app that will allow Seattle, Bellingham and Mt. Vernon pedestrians generate customized walking directions tuned to personal mobility preferences. Users can request routes from A to B that include only crossings with “curb cuts” that allow strollers and wheelchairs to easily pass, or only sidewalks within a certain steepness range personalized to the user.

# Download and Access Links
iOS and Android: https://linktr.ee/jial8
Web: https://www.accessmap.io 

# Wiki Structure
Note: the main important files/folders are listed below.
```markdown
├── README.md
├── design (Design Documentation for AccessMap)
├── mobile (Mobile-Specific Documentation)
│   ├── developer-guide.md
│   ├── quickstart.md
│   ├── release-docs (anything to do with publishing)
│   ├── technical-docs (code-specific notes)
│   └── user-guide.md (non-technical user tutorial)
└── web (Web Browser Application Documentation)
```

# List of Repos
- [accessmap](https://github.com/AccessMap/accessmap) (web application)
- [accessmap-react-native](https://github.com/AccessMap/accessmap-react-native) (Codebase for our React Native mobile app)
- [accessmap-backend](https://github.com/AccessMap/accessmap-backend) (Codebase for our TypeScript NodeJS backend server that handles user profiles)
- TODO add more here