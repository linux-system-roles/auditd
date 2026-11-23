Changelog
=========

[1.2.0] - 2026-11-23
--------------------

### New Features

- feat: add kernel audit enablement and checking (#68)
- feat: Add SLE16 support (#77)
- feat: Handle reboot for transactional update systems (#84)

### Bug Fixes

- fix: load audit rules right away and restore them if the load fails (#91)

### Other Changes

- ci: no CI test by default - implement slash commands for CI tests [citest_skip] (#70)
- ci: ansible-test-milestone is now version 2.23 - update sanity ignore files (#71)
- ci: allow lsr org members to run ci tests (#72)
- ci: Run Dependabot monthly and group changes in a single PR (#75)
- ci: bump tox-lsr version 3.21.0, myrotvorets/set-commit-status-action, support leap-16.0 (#76)
- refactor: role depends on fedora.linux_system_roles (#78)
- test: check invalid inputs for correct error message (#79)
- ci: use shared actions and lock workflow dependencies (#80)
- ci: use shared actions and lock workflow dependencies (#81)
- ci: Use order 10 for centos vault task so that it runs first (#82)
- docs: document auditd test plugins (#83)
- docs: add AI policy; update setup-python, codeql actions (#85)
- ci: retry centos vault repo failures using new package_retry yum/dnf plugin (#86)
- docs: tag markdown plain text blocks correctly (#87)
- ci: Use a fixed 5 minute backoff for CentOS vault repos (#88)
- ci: support Fedora 45, Ansible 2.22; drop Fedora 43 (#89)
- ci: use ubuntu 24.04 for test envs that use py39 (#90)
- ci: use ubuntu 26.04 with podman 5.x and disable apparmor restriction (#92)
- docs: remove extra blank lines from .coderabbit.yaml (#93)
- ci: update tox-lsr for support for tests/module_utils (#94)

[1.1.1] - 2026-09-17
--------------------

### Other Changes

- ci: use commit hash for github action, add persist-credentials false [citest_skip] (#26)
- ci: refactor build_docs so that pandoc runs in isolated read-only job [citest_skip] (#30)
- ci: use exact match for systemroller instead of contains (#31)
- ci: no citest by default - trigger by comment or label (#34)
- ci: trigger only by comment - same as tft (#41)
- ci: use nicely formatted condition and name (#43)
- ci: try with citest_ansible-lint (#45)
- ci: try with pr labeled event (#47)
- ci: debug pr label failure (#49)
- ci: debug each condition (#51)
- ci: debug why pr author_association fails (#53)
- ci: no citest by default - require comment or label (#55)
- ci(build_docs): fix pandoc container syntax [citest_skip] (#57)
- ci: [citest_skip] Bump actions/download-artifact from 7.0.0 to 8.0.1 (#58)
- ci: [citest_skip] Bump myrotvorets/set-commit-status-action from 2774e1f040c82ed70a76b4b5cd53bb11ffaedd0a to c0f880c99d91381c6fdb97726f03feb8004409b4 (#59)
- ci: [citest_skip] Bump codespell-project/actions-codespell from 2.1 to 2.2 (#60)
- refactor: Relax collection constraints, gate vendored modules by python version, update ci versions [citest_skip] (#62)
- docs: remove duplicate filter conditions in example (#63)
- ci: do not run ci tests by default, require citest comment or label [citest_skip] (#65)
- ci: replace weekly_ci with periodic_ci, stagger schedules [citest_skip] (#66)
- ci: update status when action triggered by issue comment (#67)

[1.1.0] - 2026-08-06
--------------------

### New Features

- feat: Write roles fingerprints to /var/log/sysroles.jsonl [citest_skip] (#24)

### Other Changes

- ci: Bump actions/checkout from 6 to 7 (#17)
- ci: Use our own pr_title_lint.py instead of NPM commitlint [citest_skip] (#18)
- ci: bump tox-lsr version to 3.20.0 to fix tox 4.58 api breakage [citest_skip] (#19)
- ci: Add support for Fedora 44 and drop Fedora 42 - use ansible-core 2.21 [citest_skip] (#21)
- ci: Bump actions/setup-python from 6 to 7 (#22)
- ci: ensure dependabot updates do not invoke ci tests [citest_skip] (#23)

[1.0.2] - 2026-06-24
--------------------

### Other Changes

- refactor: use ansible.posix 2.1.X for EL7 compatibility [citest_skip] (#10)
- ci: Add config file for CodeRabbit with custom rules (#11)
- ci: Skip reviews for PRs with [citest_skip] in the title (#12)
- test: use ausearch --input-logs when running on localhost (#13)
- chore: add ostree packages-runtime.txt [citest_skip] (#14)
- test: use openat instead of open - supported on all arches - skip b32 on ppc64le (#15)

[1.0.1] - 2026-05-08
--------------------

### Other Changes

- refactor: use min_ansible_version 2.9 to be consistent with other roles [citest_skip] (#8)

[1.0.0] - 2026-05-07
--------------------

### New Features

- feat: auditd - new role - initial commit (#1)
- feat: add role fingerprints to syslog (#6)

### Other Changes

- ci: add ci workflows and config files (#2)
- ci: Bump actions/github-script from 8 to 9 (#3)

