Do this to generate your change history

    git log --pretty=format:'  * [%h](https://github.com/pact-foundation/pact-go/commit/%h) - %s (%an, %ad)' vX.Y.Z..HEAD | egrep -v "wip(:|\()" | grep -v "docs(" | grep -v "chore(" | grep -v Merge | grep -v "test("

### 0.0.8 (15th July 2017)

  * [e1aaa4f](https://github.com/pact-foundation/pact-go/commit/e1aaa4f) - fix(test): add consumer test for #36 (Matt Fellows, Mon Jun 26 18:46:24 2017 +1000)
  * [cf10aa6](https://github.com/pact-foundation/pact-go/commit/cf10aa6) - fix: allow test within pact.Verify() to fail build (Matt Fellows, Wed Jun 21 00:02:44 2017 +1000)
  * [5a6855a](https://github.com/pact-foundation/pact-go/commit/5a6855a) - feat(upgrade): upgrade to provider verifier v1.1.2 (Matt Fellows, Mon Jun 12 21:31:58 2017 +1000)
  * [bcdf7b2](https://github.com/pact-foundation/pact-go/commit/bcdf7b2) - fix(log): incorrectly writing stderr to INFO and vice versa. Fixes #10 (Matt Fellows, Fri Jun 2 13:04:24 2017 +1000)
  * [4d838dc](https://github.com/pact-foundation/pact-go/commit/4d838dc) - feat(upgrade): upgrade to provider verifier v1.1.1 (Matt Fellows, Thu Jun 1 14:38:21 2017 +1000)
  * [05b3e65](https://github.com/pact-foundation/pact-go/commit/05b3e65) - feat(verification): remove ProviderStatesURL during verification (Matt Fellows, Thu Jun 1 13:43:36 2017 +1000)
  * [9002469](https://github.com/pact-foundation/pact-go/commit/9002469) - feat(upgrade): upgrade mock service to 2.1.0 (Matt Fellows, Mon May 15 08:57:36 2017 +1000)

### 0.0.7 (20th May 2017)

  * [9f2c7fe](https://github.com/pact-foundation/pact-go/commit/9f2c7fe) - feat(pactwritemode): allow user to set pact write mode.Fixes #30 (Matt Fellows, Fri May 12 10:53:32 2017 +1000)
  * [50d6b90](https://github.com/pact-foundation/pact-go/commit/50d6b90) - fix(providerstate): make provider state serialisation spec compliant #16 (Matt Fellows, Thu May 11 20:46:22 2017 +1000)

### 0.0.6 (12th May 2017)

  * [9f2c7fe](https://github.com/pact-foundation/pact-go/commit/9f2c7fe) - feat(pactwritemode): allow user to set pact write mode.Fixes #30 (Matt Fellows, Fri May 12 10:53:32 2017 +1000)
  * [50d6b90](https://github.com/pact-foundation/pact-go/commit/50d6b90) - fix(providerstate): make provider state serialisation spec compliant #16 (Matt Fellows, Thu May 11 20:46:22 2017 +1000)

### 0.0.5 (10th May 2017)

  * [ee36bff](https://github.com/pact-foundation/pact-go/commit/ee36bff) - feat(verification): publish verification results to broker (Matt Fellows, Tue May 9 15:02:05 2017 +1000)

### 0.0.4 (2nd May 2017)

  * [e89585e](https://github.com/pact-foundation/pact-go/commit/e89585e) - fix(verify) prevent crash when calling VerifyProvider() (Timothy Jones, Mon May 1 17:46:13 2017 +1000)
  * [8819608](https://github.com/pact-foundation/pact-go/commit/8819608) - feat(ruby): clean ruby stack trace in pact provider verification failures #19 (Matt Fellows, Sun Apr 30 14:25:55 2017 +1000)
  * [483d134](https://github.com/pact-foundation/pact-go/commit/483d134) - feat(verify): allow user to increase verbosity of verification process (Matt Fellows, Fri Apr 28 18:49:01 2017 +1000)
  * [c8f8c1b](https://github.com/pact-foundation/pact-go/commit/c8f8c1b) - feat(ruby): update to latest ruby dependencies 2.0.0 and 0.0.13 respectively (Matt Fellows, Fri Apr 28 18:44:53 2017 +1000)
  * [f1ee33c](https://github.com/pact-foundation/pact-go/commit/f1ee33c) - feat(e2e): run e2e tests in wercker builds. Fixes #20 (Matt Fellows, Fri Apr 28 18:43:53 2017 +1000)
  * [33a0434](https://github.com/pact-foundation/pact-go/commit/33a0434) - feat(fix): don't start mock server if not required. Fixes #21 (Matt Fellows, Fri Apr 28 17:07:39 2017 +1000)
  * [cb4d811](https://github.com/pact-foundation/pact-go/commit/cb4d811) - fix(windows): cleanup logging for windows service manager (Matt Fellows, Wed Feb 22 21:52:42 2017 +1100)
  * [d214c54](https://github.com/pact-foundation/pact-go/commit/d214c54) - fix: increased timeout to reduce likelihood of intermittent failure #11 (Matt Fellows, Tue Feb 21 21:42:36 2017 +1100)
  * [0bcca95](https://github.com/pact-foundation/pact-go/commit/0bcca95) - fix(windows): ability to pass in network and address into Pact DSL (Matt Fellows, Tue Feb 21 18:33:00 2017 +1100)
  * [e97226d](https://github.com/pact-foundation/pact-go/commit/e97226d) - fix(windows): windows leaves persistent connection open to Ruby, forcibly close 3s after interrupt  #9 (Matt Fellows, Tue Feb 21 00:17:46 2017 +1100)
  * [3616976](https://github.com/pact-foundation/pact-go/commit/3616976) - fix(windows): split pact verification CLI arg tuples into individual elements #9 (Matt Fellows, Mon Feb 20 18:12:04 2017 +1100)
  * [0dad9cc](https://github.com/pact-foundation/pact-go/commit/0dad9cc) - fix(windows): split mock service CLI arg tuples into individual elements #9 (Matt Fellows, Mon Feb 20 18:04:27 2017 +1100)
  * [2c6c84d](https://github.com/pact-foundation/pact-go/commit/2c6c84d) - fix(windows): update default pact output path (Matt Fellows, Mon Feb 20 17:53:04 2017 +1100)
  * [a963058](https://github.com/pact-foundation/pact-go/commit/a963058) - fix(windows): set default network to 'tcp' #9 (Matt Fellows, Mon Feb 20 17:49:39 2017 +1100)
  * [c84afad](https://github.com/pact-foundation/pact-go/commit/c84afad) - fix(windows): make log/pact output paths os-specific #9 (Matt Fellows, Mon Feb 20 17:47:58 2017 +1100)
  * [e586b1d](https://github.com/pact-foundation/pact-go/commit/e586b1d) - fix(windows): allow pact client to specify the network and address of daemon #9 (Matt Fellows, Mon Feb 20 17:46:54 2017 +1100)
  * [5c89b30](https://github.com/pact-foundation/pact-go/commit/5c89b30) - feat(daemon): allow user to specify network listen details for daemon (Matt Fellows, Mon Feb 20 08:59:49 2017 +1100)
  * [52b7e19](https://github.com/pact-foundation/pact-go/commit/52b7e19) - feat(examples): add vanilla golang ServeMux, update docs (Matt Fellows, Mon Sep 26 22:09:45 2016 +1000)

### 0.0.3 (30 April 2017)

  * [8819608](https://github.com/pact-foundation/pact-go/commit/8819608) - feat(ruby): clean ruby stack trace in pact provider verification failures #19 (Matt Fellows, Sun Apr 30 14:25:55 2017 +1000)
  * [483d134](https://github.com/pact-foundation/pact-go/commit/483d134) - feat(verify): allow user to increase verbosity of verification process (Matt Fellows, Fri Apr 28 18:49:01 2017 +1000)
  * [33a0434](https://github.com/pact-foundation/pact-go/commit/33a0434) - feat(fix): don't start mock server if not required. Fixes #21 (Matt Fellows, Fri Apr 28 17:07:39 2017 +1000)
  * [cb4d811](https://github.com/pact-foundation/pact-go/commit/cb4d811) - fix(windows): cleanup logging for windows service manager (Matt Fellows, Wed Feb 22 21:52:42 2017 +1100)
  * [d214c54](https://github.com/pact-foundation/pact-go/commit/d214c54) - fix: increased timeout to reduce likelihood of intermittent failure #11 (Matt Fellows, Tue Feb 21 21:42:36 2017 +1100)
  * [0bcca95](https://github.com/pact-foundation/pact-go/commit/0bcca95) - fix(windows): ability to pass in network and address into Pact DSL (Matt Fellows, Tue Feb 21 18:33:00 2017 +1100)
  * [e97226d](https://github.com/pact-foundation/pact-go/commit/e97226d) - fix(windows): windows leaves persistent connection open to Ruby, forcibly close 3s after interrupt  #9 (Matt Fellows, Tue Feb 21 00:17:46 2017 +1100)
  * [3616976](https://github.com/pact-foundation/pact-go/commit/3616976) - fix(windows): split pact verification CLI arg tuples into individual elements #9 (Matt Fellows, Mon Feb 20 18:12:04 2017 +1100)
  * [0dad9cc](https://github.com/pact-foundation/pact-go/commit/0dad9cc) - fix(windows): split mock service CLI arg tuples into individual elements #9 (Matt Fellows, Mon Feb 20 18:04:27 2017 +1100)
  * [2c6c84d](https://github.com/pact-foundation/pact-go/commit/2c6c84d) - fix(windows): update default pact output path (Matt Fellows, Mon Feb 20 17:53:04 2017 +1100)
  * [a963058](https://github.com/pact-foundation/pact-go/commit/a963058) - fix(windows): set default network to 'tcp' #9 (Matt Fellows, Mon Feb 20 17:49:39 2017 +1100)
  * [c84afad](https://github.com/pact-foundation/pact-go/commit/c84afad) - fix(windows): make log/pact output paths os-specific #9 (Matt Fellows, Mon Feb 20 17:47:58 2017 +1100)
  * [e586b1d](https://github.com/pact-foundation/pact-go/commit/e586b1d) - fix(windows): allow pact client to specify the network and address of daemon #9 (Matt Fellows, Mon Feb 20 17:46:54 2017 +1100)
  * [5c89b30](https://github.com/pact-foundation/pact-go/commit/5c89b30) - feat(daemon): allow user to specify network listen details for daemon (Matt Fellows, Mon Feb 20 08:59:49 2017 +1100)
  * [b82cb86](https://github.com/pact-foundation/pact-go/commit/b82cb86) - fix(verify): allow verification process to pull pacts from an https broker (Matt Fellows, Fri Jul 15 08:07:31 2016 +1000)
  * [9c1f206](https://github.com/pact-foundation/pact-go/commit/9c1f206) - refactor(review): improve API and reduce noise (Matt Fellows, Sun Jul 3 22:53:59 2016 +1000)

### 0.0.2 (1 July 2016)

  * [4e1539b](https://github.com/pact-foundation/pact-go/commit/4e1539b) - feature(example): add logout to Go Kit consumer (Matt Fellows, Wed Jun 15 08:58:45 2016 +1000)
  * [0cc51cd](https://github.com/pact-foundation/pact-go/commit/0cc51cd) - feat(example): dded login failure to Go Kit example (Matt Fellows, Wed Jun 15 08:50:53 2016 +1000)
  * [70c4469](https://github.com/pact-foundation/pact-go/commit/70c4469) - feat(example): simple bootstrap form for Go Kit UI (Matt Fellows, Tue Jun 14 21:30:49 2016 +1000)
  * [ff5e832](https://github.com/pact-foundation/pact-go/commit/ff5e832) - feat(publish): automatically write pact file on shutdown/teardown (Matt Fellows, Tue Jun 14 01:41:17 2016 +1000)
  * [0001703](https://github.com/pact-foundation/pact-go/commit/0001703) - feat(example): create example Go Kit microservice Pact testing (Matt Fellows, Sun Jun 12 10:26:21 2016 +1000)
  * [33f5394](https://github.com/pact-foundation/pact-go/commit/33f5394) - refactor(states): add types for provider state testing (Matt Fellows, Sun Jun 12 10:25:14 2016 +1000)
  * [ea2c807](https://github.com/pact-foundation/pact-go/commit/ea2c807) - feat(writepact): allow client to control when pact file is written (Matt Fellows, Sat Jun 11 23:18:26 2016 +1000)
  * [879a3b4](https://github.com/pact-foundation/pact-go/commit/879a3b4) - fix(daemon): fix daemon unable to find mock + verification service when called from $PATH (Matt Fellows, Sat Jun 11 13:01:25 2016 +1000)
  * [ef33b71](https://github.com/pact-foundation/pact-go/commit/ef33b71) - refactor(daemon): cleanup pointer usage in daemon code (Matt Fellows, Sat Jun 11 08:12:35 2016 +1000)
  * [7f64f9c](https://github.com/pact-foundation/pact-go/commit/7f64f9c) - feat(publish): publish pacts to a broker (Matt Fellows, Fri Jun 10 20:44:23 2016 +1000)

### 0.0.1 (7 June 2016)

  * [3255d7f](https://github.com/pact-foundation/pact-go/commit/3255d7f) - feat(verifier): complete implementation of pact verification feature (Matt Fellows, Mon Jun 6 22:41:44 2016 +1000)
  * [db83055](https://github.com/pact-foundation/pact-go/commit/db83055) - feat(logging): standardise log and output messages (Matt Fellows, Sun Jun 5 14:25:01 2016 +1000)
  * [7c3c70b](https://github.com/pact-foundation/pact-go/commit/7c3c70b) - feat(consumerdsl): working v1 consumer DSL interface (Matt Fellows, Sat Jun 4 18:52:38 2016 +1000)
  * [3b859cf](https://github.com/pact-foundation/pact-go/commit/3b859cf) - test(daemon): RPC Client error tests (Matt Fellows, Sat Jun 4 09:38:58 2016 +1000)
  * [7d8a0fd](https://github.com/pact-foundation/pact-go/commit/7d8a0fd) - test(service): remove need for a running pact mock service in tests (Matt Fellows, Fri Jun 3 22:05:12 2016 +1000)
  * [98b7c57](https://github.com/pact-foundation/pact-go/commit/98b7c57) - test(service): improved test coverage for services (Matt Fellows, Fri Jun 3 21:08:25 2016 +1000)
  * [c3f11e1](https://github.com/pact-foundation/pact-go/commit/c3f11e1) - test(daemon): coverage for shutting down the daemon via RPC (Matt Fellows, Fri Jun 3 08:19:35 2016 +1000)
  * [83c75c2](https://github.com/pact-foundation/pact-go/commit/83c75c2) - test(daemon): RPC client testing (Matt Fellows, Thu Jun 2 21:17:28 2016 +1000)
  * [3c71bba](https://github.com/pact-foundation/pact-go/commit/3c71bba) - test(service): initial service test coverage (Matt Fellows, Wed Jun 1 21:09:27 2016 +1000)
  * [27d50d4](https://github.com/pact-foundation/pact-go/commit/27d50d4) - test(daemon): RPC style tests to ensure client can work (Matt Fellows, Wed Jun 1 08:47:20 2016 +1000)
  * [5ccfb64](https://github.com/pact-foundation/pact-go/commit/5ccfb64) - test(daemon): working tests with RPC integration-style tests (Matt Fellows, Tue May 31 18:36:22 2016 +1000)
  * [3f764a6](https://github.com/pact-foundation/pact-go/commit/3f764a6) - test(daemon): working daemon tests (Matt Fellows, Tue May 31 10:30:53 2016 +1000)
  * [24e7c9b](https://github.com/pact-foundation/pact-go/commit/24e7c9b) - test(daemon): improved daemon test coverage (Matt Fellows, Tue May 31 07:30:17 2016 +1000)
  * [345cd9f](https://github.com/pact-foundation/pact-go/commit/345cd9f) - test(daemon): daemon testing (Matt Fellows, Mon May 30 22:41:15 2016 +1000)
  * [8c13832](https://github.com/pact-foundation/pact-go/commit/8c13832) - test(daemon): improved daemon test coverage for listing servers (Matt Fellows, Wed May 25 22:10:42 2016 +1000)
  * [2b5b06e](https://github.com/pact-foundation/pact-go/commit/2b5b06e) - feat(consumerdsl): initial shell for Pact Go (Matt Fellows, Sat May 21 13:27:21 2016 +1000)
