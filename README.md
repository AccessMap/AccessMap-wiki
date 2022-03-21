# AccessMap Wiki Summary
AccessMap provides a customizable pedestrian navigation experience on web, Android, and iOS. Explore your city and get helpful routes that fit your mobility profile.

There are many apps and sites to help people navigate by car: Waze, HERE, Apple Maps, Google Maps; all these apps offer some semblance of 'pedestrian' directions, but make gross assumptions about what hills you can take, how speedy you will be, what is a 'safe' walking or rolling environment, and many don't even provide basic information about whether or not there's a sidewalk there. AccessMap, previously a web application produced by the [Taskar Center for Accessible Technology](https://tcat.cs.washington.edu/) is bringing mobility equity to pedestrians by improving and customizing walking/rolling routing.

**December 2021 Release**: For International Day acknowledging Persons with Disabilities (Dec 3 #IDPWD2021) the group is releasing the mobile app that will allow Seattle, Bellingham and Mt. Vernon pedestrians generate customized walking directions tuned to personal mobility preferences. Users can request routes from A to B that include only crossings with “curb cuts” that allow strollers and wheelchairs to easily pass, or only sidewalks within a certain steepness range personalized to the user.

# Download and Access Links
iOS and Android: https://linktr.ee/jial8
Web: https://www.accessmap.io 

# Wiki Structure
Note: only the main important files/folders are listed below.
```markdown
├── backend (profiles, routing, etc)
├── design (user interface, Figma, etc)
├── mobile
│   ├── developer-guide.md (technical quickstart)
│   ├── quickstart.md
│   ├── release-docs (anything related to pushing to production)
│   │   ├── publishing.md (how to push AccessMap to production)
│   │   └── release-notes (make a release notes per official release)
│   ├── technical-docs (anything code-related)
│   │   ├── TODO.md (action items)
│   │   ├── analytics (how the app gathers data)
│   │   ├── authentication (new feature: user login)
│   │   ├── map
│   │   └── ui
│   └── user-guide.md (non-technical how-to-use AccessMap for Users)
└── web (accessmap.io)
```

# Active Repos
- [accessmap](https://github.com/AccessMap/accessmap) (web application, production)
- [accessmap-react-native](https://github.com/AccessMap/accessmap-react-native) (Codebase for our React Native mobile app)
- [accessmap-backend](https://github.com/AccessMap/accessmap-backend) (Codebase for our TypeScript NodeJS backend server that handles user profiles)
- [accessmap-incremental](https://github.com/AccessMap/accessmap-incremental) (tech demo for new routing)
- TODO add more here.

# Archived Repos
TODO add here.

# Development Team
- Anat Caspi - Co-founder
- [Nick Bolten](https://github.com/nbolten) - Co-founder, Wizard
- [AryaGJ18](https://github.com/AryaGJ18) - 
- [Samuel Felker](https://github.com/sfelker) - Developer
- [Sumit Mukherjee](https://github.com/mukhes3) - 
- [Kristin Ann Tufte](https://github.com/kristinann)
- [Andrew Tan](https://github.com/Andrew-Tan) - Developer
- [Eric Yeh](https://github.com/yehric2018) - Developer (Web, React Native)
- [Chris Cheng]() - UX Designer
- [Julia Beckwith](https://github.com/jsbeckwith) - Developer (Unweaver)
- [Jay Lin](https://github.com/JetPlaneJJ) - Developer (React Native, Profiles-backend)
- [Renusree Chittella]() - Developer (E-mission)
- [David Hyun](https://github.com/DavyHyun) - Developer (React Native)
