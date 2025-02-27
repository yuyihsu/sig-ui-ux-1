## Asset Browser Project 

An Asset Browser (AB) is a critical function of any game engine. Allowing external tooling such as file manipulation, file creation, and file management to be done in a centralized place, inside the game engine. Not forcing the user to rely on windows explorer to manage this experience outside the editor. Over the past several years many of our customers have told us that our AB experience is awful compared to all of the other game engines out there. Unfortunately, this bit of feedback is true. We lack many of the most fundamental functionality to make asset management usable within the editor.  So, our intention is to fix this. Setting our intentions to be at least in parity with the 3 other major game engines out there (Godot, Unity, and Unreal). In short, if all 3 other game engines support the same feature across all of their editors. We should be considering this as a feature we want to explorer in O3DE. A good calibration for our team is to remember that Godot is also another open source game engine which only takes support from the community. In their circumstance, they have listened to their customers and have used their limited resources to work on a better AB experience. This is because they have learned that a good AB is critical to a game engine success.
About this project

O3DE has been working hard on putting together some great new improvements for our asset management system, specifically focusing on Asset Browser and Asset Processor. In this pipeline we are taking a longer term more sequential approach to this enhancements that will roll out over the next 18 months. Some of these changes will even be seen in the next release. All of these incremental changes are coming together by user feedback and competitive analysis.

Customers have told us through RTE and in customer interviews that our Asset Browser system is lacking some fundemental features and is not up to the industry standards. We have carefully listen to this feedback, anyalized, prioritized, and created a roadmap to add or enhance these features. To accomplish this, we’ve established an Asset Browser project team, designed the workflows, and have triaged a backlog of features into 4 upcoming releases.

- **Phase 1:** File operations (coming soon) - Deleting, opening, moving, adding, duplicating, renaming and working with source control.
- **Phase 2:** Layouts and views - Three different layouts, a new detail panel, and a search bar.
- **Phase 3:** Advanced operations - expression searches, favorites, and multiple asset browser tabs.
- **Phase 4:** Asset Browser inspector panel - Detailed view about your assets and all assets associated to that asset.

### Project links
- https://github.com/orgs/o3de/projects/16/views/1

### phase 1	

| Task  | User Story| Notes |
| ------------- | ------------- |------------- |
| Delete Files in the Asset Browser Done | As a user I need the ability to delete asset from Asset Browser | Make sure it works with source control from v1. might include some kind of popup window. Do not ask me again type of question. Also way to reset it. Consult with Asset Browser - UX about querying/informing the Asset Processor and warning the user when necessary.
| Editing files in AB in the Asset Browser Done | As a user I need the ability to Edit an asset from AB (double clicking on an asset or right click > edit). This means if I click script, a 3d object, a material, a C++ file, we can determine a default launching state of each type and support an open state even if it doesn't open with O3DE. | If we don't know what application to use we should default to the window/ OS base opener application default application |
| Move Files and Folders in the Asset Browser Done | As a user I need the ability to move folder and content from one place to another within asset browser. This mean move content from here to here but also, cut and past, copy and paste.	| Right click to move folder OR hotkey. Maybe shift / alt moving copying. Check to make sure we can do shift selection. Rubberband: a square.
| Add new material in Asset Browser Done | As a user I need to be able to right click and or click on the plus button in the AB and add a new material. This should launch Material editor and already create a new material on disc for the user. User should be able to rename the asset at this point	| None |
| Add new script file (script Canvas) in Asset Browser Done | As a user I need to be able to right click and or click on the plus button in the AB and add a new script file (Script Canvas, C++, python). User should be able to rename this script and double click to launch the respective editor	| None |
|Add a new animation file in Asset Browser Done | As a user I need to be able to right click and or click on the plus button in the AB and add a new animation file. the file would be an empty animation file. User should be able to rename and then double click file to open the animation file.	|	Make new workflows might need to be assisted by the team who own that particular workflow. So this might include conversations with the animation team. We might need some kind of bus call from each team. We would need some kind of documentation to create new asset types. (provide hooks and docs for this)|
| Add a new Level and add new prefab in Asset Browser | As a user I need to be able to right click and or click on the plus button in the AB and add a new Level OR prefab. user should be able to rename this file	| None |	
| Folder managment inside Asset Browser (Add/Remove) Done | As a user I need a way to do folder management inside AB. This includes adding folders, remove folders, (hind folder from AB - maybe unrelated assets you don't want to include) |	This should work with perforce/version control. We might also need some kind of show hidden folder button. |
| Duplicate files or folders inside Asset Browser. Done | As a user I need the ability to duplicate a file or folder inside AB.	|	This should work with perforce/version control.|
|Rename files and folders in the Asset Browser Done | As a user I need the ability to rename a file or folder inside AB	| This should work with perforce/version control. |
| Drag and drop from AB to the editor In Progress | As a user I need to refine the drag and drop target area for my cursor | None |
