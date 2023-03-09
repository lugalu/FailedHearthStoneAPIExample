# HearthStone API Example
The Purpose of this repo was studying making API calls with both default Swift URLRequest and AlamoFire Requests, and also use for the first time Carthage and XCode generation, due to a number of problems and work-arounds needed to make this work I decided to stop using both of them and instead of deleting the entire repo I decided as a public archive to have a documentation on my bad combination and implementation.

## Problems Encountered
Here is the list of bugs that made me take this route with the repo:
- Carthage still can't build with frameworks that have multiple builds for 86x and arm64 architecture, needs a custom script found in the documentation of [carthage project](https://github.com/Carthage/Carthage/blob/master/Documentation/Xcode12Workaround.md);

- [Xcode generation](https://github.com/yonaskolb/XcodeGen) was creating build files without multiple base configurations like missing default Executable file, build name, version, and others, also it didn't import carthage frameworks correctly;

I could spend more time fixing this problems but I felt that would be a huge waste of time, over engineering and wouldn't help me learn that much.

So use this repo as a warning or guide to fix problems that you may have.
