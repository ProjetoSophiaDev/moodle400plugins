# moodle400plugins
Moodle MOOC Plugins

## Upgrade Submodules
```bash
git submodule update --remote
```
## Disable Notifications

```php
// Moodle configuration file
 
// Use the following flag to completely disable the installation of plugins
// (new plugins, available updates and missing dependencies) and related
// features (such as cancelling the plugin installation or upgrade) via the
// server administration web interface.
$CFG->disableupdateautodeploy = true;
// Disabling update notifications
$CFG->disableupdatenotifications = true;

// Some administration options allow setting the path to executable files. This can
// potentially cause a security risk. Set this option to true to disable editing
// those config settings via the web. They will need to be set explicitly in the
// config.php file
$CFG->preventexecpath = true;

// Force result of checks used to determine whether a site is considered "public" or not (such as for site registration).
$CFG->site_is_public = false;
```
## References
https://www.vogella.com/tutorials/GitSubmodules/article.html

## Jenkins
https://jenkins.adrianoruseler.com/view/Sophia/job/Sophia-MDLDevUpdate/

## Plugins List

```bash
mkdir moodle
cd moodle
```
- https://github.com/danmarsden/moodle-mod_attendance/
```bash
git submodule add -b MOODLE_400_STABLE https://github.com/danmarsden/moodle-mod_attendance.git mod/attendance
```
- https://github.com/markn86/moodle-mod_customcert
```bash
git submodule add -b MOODLE_311_STABLE https://github.com/markn86/moodle-mod_customcert.git mod/customcert
```
- https://github.com/FMCorz/moodle-block_xp
```bash
git submodule add -b master https://github.com/FMCorz/moodle-block_xp.git blocks/xp
```
- https://github.com/deraadt/moodle-block_completion_progress
```bash
git submodule add -b master https://github.com/deraadt/moodle-block_completion_progress.git blocks/completion_progress
```
- https://github.com/ndunand/moodle-mod_choicegroup
```bash
git submodule add -b master https://github.com/ndunand/moodle-mod_choicegroup.git mod/choicegroup
```
- https://github.com/dthies/moodle-atto_fullscreen
```bash
git submodule add -b master https://github.com/dthies/moodle-atto_fullscreen.git lib/editor/atto/plugins/fullscreen
```
- https://github.com/frankkoch/moodle-mod_studentquiz
```bash
git submodule add -b main https://github.com/frankkoch/moodle-mod_studentquiz.git mod/studentquiz
```
- https://github.com/mikasmart/moodle-report_benchmark
```bash
git submodule add -b master https://github.com/mikasmart/moodle-report_benchmark.git report/benchmark
```
- https://github.com/davosmith/moodle-checklist
```bash
git submodule add -b master https://github.com/davosmith/moodle-checklist.git mod/checklist
```
- https://github.com/bostelm/moodle-mod_scheduler
```bash
 git submodule add -b master https://github.com/bostelm/moodle-mod_scheduler.git mod/scheduler
```
- https://github.com/moodleuulm/moodle-local_sandbox
```bash
git submodule add -b master https://github.com/moodleuulm/moodle-local_sandbox.git local/sandbox
```
- https://moodle.org/plugins/block_dedication
```bash
git submodule add -b MOODLE_30_STABLE https://bitbucket.org/ciceidev/moodle_block_dedication.git blocks/dedication
```
- https://github.com/mudrd8mz/moodle-mod_subcourse
```bash
git submodule add -b main https://github.com/mudrd8mz/moodle-mod_subcourse.git mod/subcourse
```
- https://github.com/academic-moodle-cooperation/moodle-mod_publication
```bash
git submodule add -b MOODLE_311_STABLE https://github.com/academic-moodle-cooperation/moodle-mod_publication.git mod/publication
```
- https://moodle.org/plugins/availability_relativedate
```bash
git submodule add -b main https://github.com/ewallah/moodle-availability_relativedate.git availability/condition/relativedate
```
- https://bitbucket.org/dw8/moodle-format_tiles
```bash
git submodule add -b master https://bitbucket.org/dw8/moodle-format_tiles.git course/format/tiles
```
- https://github.com/brandaorodrigo/moodle-format_buttons
```bash
git submodule add -b master https://github.com/brandaorodrigo/moodle-format_buttons.git course/format/buttons
```
- https://github.com/cellule-tice/moodle-format_collapsibletopics
```bash
git submodule add -b master https://github.com/cellule-tice/moodle-format_collapsibletopics.git course/format/collapsibletopics
```
- https://github.com/jcrodriguez-dis/moodle-mod_vpl
```bash
git submodule add -b V3.5.0 https://github.com/jcrodriguez-dis/moodle-mod_vpl.git mod/vpl
```
- https://gricad-gitlab.univ-grenoble-alpes.fr/bizarda/moodle-qtype_vplquestion
```bash
git submodule add -b master https://gricad-gitlab.univ-grenoble-alpes.fr/bizarda/moodle-qtype_vplquestion.git question/type/vplquestion
```
- https://github.com/michael-milette/moodle-filter_filtercodes
```bash
git submodule add -b master https://github.com/michael-milette/moodle-filter_filtercodes.git /filter/filtercodes
```
- https://github.com/trampgeek/moodle-qtype_coderunner
```bash
git submodule add -b master https://github.com/trampgeek/moodle-qtype_coderunner.git question/type/coderunner
git submodule add -b master https://github.com/trampgeek/moodle-qbehaviour_adaptive_adapted_for_coderunner.git question/behaviour/adaptive_adapted_for_coderunner
```
- https://github.com/h5p/h5p-moodle-plugin
```bash
git submodule add -b stable https://github.com/h5p/h5p-moodle-plugin.git mod/hvp
cd mod/hvp
git submodule update --init
```
- https://github.com/moodlehq/moodle-tool_migratehvp2h5p
```bash
git submodule add -b master https://github.com/moodlehq/moodle-tool_migratehvp2h5p.git admin/tool/migratehvp2h5p
```
- https://github.com/moodleou/moodle-qtype_pmatch
```bash
git submodule add -b main https://github.com/moodleou/moodle-qtype_pmatch.git question/type/pmatch
```

- https://github.com/moodleou/moodle-qtype_varnumericset
```bash
git submodule add -b main https://github.com/moodleou/moodle-qtype_varnumericset.git question/type/varnumericset
```
- https://github.com/moodleou/moodle-qtype_varnumeric
```bash
git submodule add -b main https://github.com/moodleou/moodle-qtype_varnumeric.git question/type/varnumeric
```

- https://github.com/moodleou/moodle-editor_ousupsub/
```bash
git submodule add -b main https://github.com/moodleou/moodle-editor_ousupsub.git lib/editor/ousupsub
```
- https://github.com/moodleou/moodle-qtype_varnumunit
```bash
git submodule add -b main https://github.com/moodleou/moodle-qtype_varnumunit.git question/type/varnumunit
```

## TODO
- https://github.com/bdaloukas/moodle-mod_game
```bash
 git submodule add -b MOODLE_20_STABLE https://github.com/bdaloukas/moodle-mod_game.git mod/game
```
## Error


## Removed
- https://github.com/jleyva/moodle-block_configurablereports
```bash
git submodule add -b MOODLE_36_STABLE https://github.com/jleyva/moodle-block_configurablereports.git blocks/configurable_reports
```

## Themes List

- https://github.com/lmsace/eguru

```bash
git submodule add -b v311 https://github.com/ProjetoSophiaDev/eguru.git theme/eguru
```

## How to remove a submodule
```bash
SUBMPATH="moodle/path/to/submodule"
git submodule deinit $SUBMPATH
git rm $SUBMPATH
git commit -m "Removed submodule $SUBMPATH"
rm -rf .git/modules/$SUBMPATH
git push
```

```bash
git submodule add -b branch https://urltoplugin.git path/to/submodule
git add .
git commit -m "Some update info here..."
git push
```
