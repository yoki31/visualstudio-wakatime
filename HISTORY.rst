
History
-------

12.0.0 (2021-08-13)
++++++++++++++++++

- Add support for 2022 preview.


11.0.0 (2021-08-09)
++++++++++++++++++

- Drop support for versions below 2015.
- It will correctly initialize asyncronously.
- Update WakaTime.Shared.ExtensionUtils dependency to v3.0.0.
- Fix uninstall process that could not find LICENSE file.


10.3.1 (2020-10-09)
++++++++++++++++++

- Get correct version of installed wakatime plugin.


10.3.0 (2020-10-01)
++++++++++++++++++

- Add new IDE events.
- Identify either debugging or building.
- Minor bug fixes.


10.2.0 (2020-02-25)
++++++++++++++++++

- Remove support for non-standalone cli.


10.1.0 (2020-02-21)
++++++++++++++++++

- Support for standalone wakatime-cli.


10.0.3 (2019-04-07)
++++++++++++++++++

- Bugfix: Prompt for api key first time plugin loaded.
- Remove disable threading config setting.
- Bugfix: Only one config instance needed for whole extension.


10.0.2 (2019-04-07)
++++++++++++++++++

- Fix missing WakaTime menu item.
  `#91 <https://github.com/wakatime/visualstudio-wakatime/pull/91>`_
- Load configs from wakatime.cfg before initializing plugin.


10.0.1 (2019-04-07)
++++++++++++++++++

- Run syncronous startup code after async initialize.


10.0.0 (2019-04-07)
++++++++++++++++++

- Load package async on startup, fixing warning about depreciated APIs.
  `#90 <https://github.com/wakatime/visualstudio-wakatime/pull/90>`_
- Prevent deadlocks when reading process output.
  `#80 <https://github.com/wakatime/visualstudio-wakatime/pull/80>`_


9.0.0 (2019-03-09)
++++++++++++++++++

- Add support for Visual Studio 2019.
  `#84 <https://github.com/wakatime/visualstudio-wakatime/pull/84>`_


8.1.0 (2018-10-27)
++++++++++++++++++

- Add setting and config to disable threading.
- Drop support for Python 2.6.


8.0.7 (2018-05-03)
++++++++++++++++++

- Support TLS 1.2 when downloading dependencies from GitHub.


8.0.6 (2017-01-16)
++++++++++++++++++

- Run wakatime-cli in low priority background process to prevent
  lagging GUI.


8.0.5 (2016-11-30)
++++++++++++++++++

- Add support for Visual Studio 2017.


8.0.4 (2016-05-03)
++++++++++++++++++

- Fix bug causing epoch timestamp to be created incorrectly as
  milliseconds instead of seconds.


8.0.3 (2016-05-01)
++++++++++++++++++

- Millisecond precision for heartbeat timestamps.


8.0.2 (2016-05-01)
++++++++++++++++++

- Fix bug causing heartbeat timestamp to be created incorrectly.


8.0.1 (2016-04-30)
++++++++++++++++++

- Minor bug fix to prevent downloading wakatime-cli when
  already have current version.


8.0.0 (2016-04-30)
++++++++++++++++++

- Queue heartbeats before sending to wakatime-cli to prevent
  from forking too many python processes.
- Improved dependency management and moved dependencies to
  AppData\WakaTime folder.


7.0.3 (2016-04-09)
++++++++++++++++++

- Prevent deleting wakatime-core when IDE started while offline.
- Make sure api key dialog prompt has focus.
- Add support for Visual Studio 15.


7.0.2 (2015-01-04)
++++++++++++++++++

- enable settings menu item even when dependency downloading fails, to allow setting a proxy


7.0.1 (2015-12-03)
++++++++++++++++++

- remove prompt before installing Python because using embeddable Python now


7.0.0 (2015-11-26)
++++++++++++++++++

- use embeddable python to prevent installing failures


6.0.0 (2015-10-10)
++++++++++++++++++

- improve detection of latest wakatime-cli version from GitHub repo
- prevent locking inside background thread
- better looking obfuscated api key


5.0.11 (2015-10-02)
++++++++++++++++++

- ask user to authorize to download Python and other improvements
- fixed issue when downloading Python and wakatime-cli using a proxy
- support simple proxy addresses without authentication


5.0.10 (2015-08-27)
++++++++++++++++++

- minor fix


5.0.9 (2015-08-25)
++++++++++++++++++

- upgrade wakatime cli to v4.1.1
- send hostname in X-Machine-Name header
- catch exceptions from pygments.modeline.get_filetype_from_buffer
- upgrade requests package to v2.7.0
- handle non-ASCII characters in import path on Windows, won't fix for Python2
- upgrade argparse to v1.3.0
- move language translations to api server
- move extension rules to api server
- detect correct header file language based on presence of .cpp or .c files named the same as the .h file


5.0.8 (2015-07-29)
++++++++++++++++++

- bug fix when setting api key for the first time


5.0.7 (2015-07-27)
++++++++++++++++++

- refactoring


5.0.6 (2015-07-22)
++++++++++++++++++

- replaced logging into ActivityLog.xml to Output Window
- more verbose logging added
- bug fix when saving proxy into config file


5.0.5 (2015-07-17)
++++++++++++++++++

- cache DTE object for getting solution name
- more verbose logging to ActivityLog.xml
- less strict python detection


5.0.4 (2015-07-01)
++++++++++++++++++

- support for VS2012 by changing the version of Microsoft.VisualStudio.Shell
- correct priority for project detection
- fix offline logging
- limit language detection to known file extensions, unless file contents has a vim modeline
- guess language using multiple methods, then use most accurate guess
- use entity and type for new heartbeats api resource schema
- upgrade wakatime cli to v4.1.0


5.0.3 (2015-06-08)
++++++++++++++++++

- look for Python binary location in Windows registry
- added debug option into SettingsForm


5.0.2 (2015-06-05)
++++++++++++++++++

- detect python binary from successful execution of python, without checking output


5.0.1 (2015-06-01)
++++++++++++++++++

- update wakatime cli to v4.0.14
- correctly log message from py.warnings module


5.0.2 (2015-06-05)
++++++++++++++++++

- detect python binary from successful execution of python, without checking output


5.0.1 (2015-06-01)
++++++++++++++++++

- update wakatime cli to v4.0.14
- correctly log message from py.warnings module


5.0.2 (2015-06-05)
++++++++++++++++++

- detect python binary from successful execution of python, without checking output


5.0.1 (2015-06-01)
++++++++++++++++++

- update wakatime cli to v4.0.14
- correctly log message from py.warnings module


5.0.0 (2015-05-30)
++++++++++++++++++

- better UX around api key and settings form
- cache Python binary location and wakatime cli location for better performance
- move wakatime cli dependency into AppData folder
- proxy field added to settings form


4.0.4 (2015-05-24)
++++++++++++++++++

- support for Visual Studio 2012


4.0.2 (2015-05-11)
++++++++++++++++++

- more changes for extension gallery


4.0.1 (2015-05-08)
++++++++++++++++++

- changes for extension gallery


4.0.0 (2015-05-08)
++++++++++++++++++

- support for Visual Studio 2015


3.0.0 (2015-04-29)
++++++++++++++++++

- refactor plugin code and fix major bugs
- support for Visual Studio 2013


2.0.2 (2014-12-21)
++++++++++++++++++

- wrap wakatime cli in quotes when executing
- use solution name as backup for project name
- send hearbeat every 2 minutes when activity detected in IDE


2.0.1 (2014-12-20)
++++++++++++++++++

- only send heartbeats when actively using IDE, not when idle
- send heartbeat asyncronously


2.0.0 (2014-12-20)
++++++++++++++++++

- fix logging
- correctly log heartbeats from IDE activity
- correctly detect Python binary
- download and install python if not already installed


1.0.0 (2014-12-18)
++++++++++++++++++

- Birth
