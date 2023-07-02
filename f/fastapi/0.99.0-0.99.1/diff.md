# Comparing `tmp/fastapi-0.99.0.tar.gz` & `tmp/fastapi-0.99.1.tar.gz`

## Comparing `fastapi-0.99.0.tar` & `fastapi-0.99.1.tar`

### file list

```diff
@@ -1,1857 +1,1858 @@
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fastapi-0.99.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi-0.99.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 fastapi-0.99.0/SECURITY.md
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 fastapi-0.99.0/requirements-docs.txt
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 fastapi-0.99.0/requirements-tests.txt
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 fastapi-0.99.0/requirements.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/dependabot.yml
--rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/DISCUSSION_TEMPLATE/questions.yml
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/ISSUE_TEMPLATE/privileged.yml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/actions/comment-docs-preview-in-pr/Dockerfile
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/actions/comment-docs-preview-in-pr/action.yml
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/actions/comment-docs-preview-in-pr/app/main.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/actions/notify-translations/Dockerfile
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/actions/notify-translations/action.yml
--rw-r--r--   0        0        0    12661 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/actions/notify-translations/app/main.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/actions/people/Dockerfile
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/actions/people/action.yml
--rw-r--r--   0        0        0    19794 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/actions/people/app/main.py
--rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/workflows/build-docs.yml
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/workflows/deploy-docs.yml
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/workflows/issue-manager.yml
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/workflows/label-approved.yml
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/workflows/notify-translations.yml
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/workflows/people.yml
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/workflows/smokeshow.yml
--rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 fastapi-0.99.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/missing-translation.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/de/mkdocs.yml
--rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/de/docs/features.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/mkdocs.yml
--rw-r--r--   0        0        0    19136 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/alternatives.md
--rw-r--r--   0        0        0    19114 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/async.md
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/benchmarks.md
--rw-r--r--   0        0        0    11702 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/contributing.md
--rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/external-links.md
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/fastapi-people.md
--rw-r--r--   0        0        0     8409 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/features.md
--rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/help-fastapi.md
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/history-design-future.md
--rw-r--r--   0        0        0    17670 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/index.md
--rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/project-generation.md
--rw-r--r--   0        0        0    13966 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/python-types.md
--rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/additional-responses.md
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/additional-status-codes.md
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/advanced-dependencies.md
--rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/async-sql-databases.md
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/async-tests.md
--rw-r--r--   0        0        0    10306 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/behind-a-proxy.md
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/conditional-openapi.md
--rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/custom-request-and-route.md
--rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/custom-response.md
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/dataclasses.md
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/events.md
--rw-r--r--   0        0        0     9748 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/extending-openapi.md
--rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/generate-clients.md
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/graphql.md
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/index.md
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/middleware.md
--rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/nosql-databases.md
--rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/openapi-callbacks.md
--rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/path-operation-advanced-configuration.md
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/response-change-status-code.md
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/response-cookies.md
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/response-directly.md
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/response-headers.md
--rw-r--r--   0        0        0    11642 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/settings.md
--rw-r--r--   0        0        0    19705 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/sql-databases-peewee.md
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/sub-applications.md
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/templates.md
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/testing-database.md
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/testing-dependencies.md
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/testing-events.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/testing-websockets.md
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/using-request-directly.md
--rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/websockets.md
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/wsgi.md
--rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/security/http-basic-auth.md
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/security/index.md
--rw-r--r--   0        0        0    11325 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/advanced/security/oauth2-scopes.md
--rw-r--r--   0        0        0    14832 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/deployment/concepts.md
--rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/deployment/deta.md
--rw-r--r--   0        0        0    28740 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/deployment/docker.md
--rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/deployment/https.md
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/deployment/index.md
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/deployment/manually.md
--rw-r--r--   0        0        0     8396 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/deployment/server-workers.md
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/deployment/versions.md
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/background-tasks.md
--rw-r--r--   0        0        0    15678 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/bigger-applications.md
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/body-fields.md
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/body-multiple-params.md
--rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/body-nested-models.md
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/body-updates.md
--rw-r--r--   0        0        0     6683 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/body.md
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/cookie-params.md
--rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/cors.md
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/debugging.md
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/encoder.md
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/extra-data-types.md
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/extra-models.md
--rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/handling-errors.md
--rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/header-params.md
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/index.md
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/metadata.md
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/middleware.md
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/path-operation-configuration.md
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/path-params-numeric-validations.md
--rw-r--r--   0        0        0     7878 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/path-params.md
--rw-r--r--   0        0        0    12188 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/query-params-str-validations.md
--rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/query-params.md
--rw-r--r--   0        0        0     6803 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/request-files.md
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/request-forms-and-files.md
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/request-forms.md
--rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/response-model.md
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/response-status-code.md
--rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/schema-extra-example.md
--rw-r--r--   0        0        0    25882 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/sql-databases.md
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/static-files.md
--rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/testing.md
--rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/dependencies/classes-as-dependencies.md
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md
--rw-r--r--   0        0        0     8941 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/dependencies/dependencies-with-yield.md
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/dependencies/global-dependencies.md
--rw-r--r--   0        0        0     6876 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/dependencies/index.md
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/dependencies/sub-dependencies.md
--rw-r--r--   0        0        0     6946 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/security/first-steps.md
--rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/security/get-current-user.md
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/security/index.md
--rw-r--r--   0        0        0     9718 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/security/oauth2-jwt.md
--rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/em/docs/tutorial/security/simple-oauth2.md
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/mkdocs.insiders.yml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/mkdocs.maybe-insiders.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/mkdocs.no-insiders.yml
--rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/mkdocs.yml
--rw-r--r--   0        0        0    19084 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/data/external_links.yml
--rw-r--r--   0        0        0    25966 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/data/github_sponsors.yml
--rw-r--r--   0        0        0    22157 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/data/people.yml
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/data/sponsors.yml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/data/sponsors_badge.yml
--rw-r--r--   0        0        0    23768 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/alternatives.md
--rw-r--r--   0        0        0    23576 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/async.md
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/benchmarks.md
--rw-r--r--   0        0        0    13506 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/contributing.md
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/external-links.md
--rw-r--r--   0        0        0     6515 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/fastapi-people.md
--rw-r--r--   0        0        0     9479 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/features.md
--rw-r--r--   0        0        0    14258 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/help-fastapi.md
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/history-design-future.md
--rw-r--r--   0        0        0    19216 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/index.md
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/newsletter.md
--rw-r--r--   0        0        0     5826 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/project-generation.md
--rw-r--r--   0        0        0    17461 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/python-types.md
--rw-r--r--   0        0        0   278060 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/release-notes.md
--rw-r--r--   0        0        0     8996 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/additional-responses.md
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/additional-status-codes.md
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/advanced-dependencies.md
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/async-sql-databases.md
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/async-tests.md
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/behind-a-proxy.md
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/conditional-openapi.md
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/custom-request-and-route.md
--rw-r--r--   0        0        0    11981 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/custom-response.md
--rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/dataclasses.md
--rw-r--r--   0        0        0     7828 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/events.md
--rw-r--r--   0        0        0    11645 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/extending-openapi.md
--rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/generate-clients.md
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/graphql.md
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/index.md
--rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/middleware.md
--rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/nosql-databases.md
--rw-r--r--   0        0        0     7934 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/openapi-callbacks.md
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/openapi-webhooks.md
--rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/path-operation-advanced-configuration.md
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/response-change-status-code.md
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/response-cookies.md
--rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/response-directly.md
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/response-headers.md
--rw-r--r--   0        0        0    14584 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/settings.md
--rw-r--r--   0        0        0    23622 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/sql-databases-peewee.md
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/sub-applications.md
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/templates.md
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/testing-database.md
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/testing-dependencies.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/testing-events.md
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/testing-websockets.md
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/using-request-directly.md
--rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/websockets.md
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/wsgi.md
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/security/http-basic-auth.md
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/security/index.md
--rw-r--r--   0        0        0    20945 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/advanced/security/oauth2-scopes.md
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/css/custom.css
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/css/termynal.css
--rw-r--r--   0        0        0    18405 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/deployment/concepts.md
--rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/deployment/deta.md
--rw-r--r--   0        0        0    35157 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/deployment/docker.md
--rw-r--r--   0        0        0    12240 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/deployment/https.md
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/deployment/index.md
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/deployment/manually.md
--rw-r--r--   0        0        0     9364 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/deployment/server-workers.md
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/deployment/versions.md
--rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/favicon.png
--rw-r--r--   0        0        0    58136 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/github-social-preview.png
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/github-social-preview.svg
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/icon-transparent-bg.png
--rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/icon-white-bg.png
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/icon-white.svg
--rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/logo-teal-vector.svg
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/logo-teal.svg
--rw-r--r--   0        0        0    51205 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/pycharm-completion.png
--rw-r--r--   0        0        0    62417 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/vscode-completion.png
--rw-r--r--   0        0        0   203390 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-01.png
--rw-r--r--   0        0        0   166992 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-02.png
--rw-r--r--   0        0        0   172943 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-03.png
--rw-r--r--   0        0        0   163423 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-04.png
--rw-r--r--   0        0        0   159869 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-05.png
--rw-r--r--   0        0        0   164838 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-06.png
--rw-r--r--   0        0        0   169968 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-07.png
--rw-r--r--   0        0        0   225993 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-01.png
--rw-r--r--   0        0        0   203644 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-02.png
--rw-r--r--   0        0        0   168628 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-03.png
--rw-r--r--   0        0        0   219429 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-04.png
--rw-r--r--   0        0        0   185116 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-05.png
--rw-r--r--   0        0        0   157113 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-06.png
--rw-r--r--   0        0        0   124827 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/concepts/image01.png
--rw-r--r--   0        0        0    10203 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/concepts/process-ram.drawio
--rw-r--r--   0        0        0    16640 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/concepts/process-ram.svg
--rw-r--r--   0        0        0    39996 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/deta/image01.png
--rw-r--r--   0        0        0    48297 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/deta/image02.png
--rw-r--r--   0        0        0    52704 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/deta/image03.png
--rw-r--r--   0        0        0    49760 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/deta/image04.png
--rw-r--r--   0        0        0    33130 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/deta/image05.png
--rw-r--r--   0        0        0   105270 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/deta/image06.png
--rw-r--r--   0        0        0    26363 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/https/https.drawio
--rw-r--r--   0        0        0    40488 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/https/https.svg
--rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/https/https01.drawio
--rw-r--r--   0        0        0    10583 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/https/https01.svg
--rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/https/https02.drawio
--rw-r--r--   0        0        0    15794 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/https/https02.svg
--rw-r--r--   0        0        0    12582 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/https/https03.drawio
--rw-r--r--   0        0        0    21549 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/https/https03.svg
--rw-r--r--   0        0        0    14291 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/https/https04.drawio
--rw-r--r--   0        0        0    23265 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/https/https04.svg
--rw-r--r--   0        0        0    15945 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/https/https05.drawio
--rw-r--r--   0        0        0    26167 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/https/https05.svg
--rw-r--r--   0        0        0    17470 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/https/https06.drawio
--rw-r--r--   0        0        0    27919 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/https/https06.svg
--rw-r--r--   0        0        0    19117 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/https/https07.drawio
--rw-r--r--   0        0        0    29659 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/https/https07.svg
--rw-r--r--   0        0        0    21427 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/https/https08.drawio
--rw-r--r--   0        0        0    33876 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/deployment/https/https08.svg
--rw-r--r--   0        0        0    74158 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/index/index-01-swagger-ui-simple.png
--rw-r--r--   0        0        0    68468 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/index/index-02-redoc-simple.png
--rw-r--r--   0        0        0    75099 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/index/index-03-swagger-02.png
--rw-r--r--   0        0        0    67572 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/index/index-04-swagger-03.png
--rw-r--r--   0        0        0    71441 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/index/index-05-swagger-04.png
--rw-r--r--   0        0        0    78842 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/index/index-06-redoc-02.png
--rw-r--r--   0        0        0     8036 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/logo-margin/logo-teal-vector.svg
--rw-r--r--   0        0        0    17680 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/logo-margin/logo-teal.png
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/logo-margin/logo-teal.svg
--rw-r--r--   0        0        0    21502 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/logo-margin/logo-white-bg.png
--rw-r--r--   0        0        0    17722 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/python-types/image01.png
--rw-r--r--   0        0        0    47799 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/python-types/image02.png
--rw-r--r--   0        0        0    42872 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/python-types/image03.png
--rw-r--r--   0        0        0    18604 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/python-types/image04.png
--rw-r--r--   0        0        0    42637 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/python-types/image05.png
--rw-r--r--   0        0        0    29581 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/python-types/image06.png
--rw-r--r--   0        0        0    37057 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/budget-insight.svg
--rw-r--r--   0        0        0    16949 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/calmcode.jpg
--rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/classiq-banner.png
--rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/classiq.png
--rw-r--r--   0        0        0   133690 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/cryptapi-banner.svg
--rw-r--r--   0        0        0   111142 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/cryptapi.svg
--rw-r--r--   0        0        0   122267 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/databento.svg
--rw-r--r--   0        0        0    38162 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/deta-banner.svg
--rw-r--r--   0        0        0    56518 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/deta.svg
--rw-r--r--   0        0        0   110000 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/docarray-top-banner.svg
--rw-r--r--   0        0        0   129629 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/docarray.svg
--rw-r--r--   0        0        0    53417 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/doist-banner.svg
--rw-r--r--   0        0        0    93166 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/doist.svg
--rw-r--r--   0        0        0    21211 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/dropbase-banner.svg
--rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/dropbase.svg
--rw-r--r--   0        0        0    10556 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/exoflare.png
--rw-r--r--   0        0        0    16235 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.png
--rw-r--r--   0        0        0    34985 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.svg
--rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/flint.png
--rw-r--r--   0        0        0    31985 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/haystack-fastapi.svg
--rw-r--r--   0        0        0   107893 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/imgwhale-banner.svg
--rw-r--r--   0        0        0   108995 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/imgwhale.svg
--rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/ines-course.jpg
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/investsuite.svg
--rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/jina-ai-banner.png
--rw-r--r--   0        0        0    26112 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/jina-ai.png
--rw-r--r--   0        0        0    42239 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/jina-banner.svg
--rw-r--r--   0        0        0   162873 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/jina-top-banner.svg
--rw-r--r--   0        0        0   220435 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/jina.svg
--rw-r--r--   0        0        0   108837 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/jina2.svg
--rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/platform-sh-banner.png
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/platform-sh.png
--rw-r--r--   0        0        0    15311 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/powens.png
--rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/striveworks-banner.png
--rw-r--r--   0        0        0    22639 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/striveworks.png
--rw-r--r--   0        0        0    34780 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/striveworks2.png
--rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/svix.svg
--rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/talkpython.png
--rw-r--r--   0        0        0    26425 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/testdriven.svg
--rw-r--r--   0        0        0    15198 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/vimso.png
--rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/sponsors/wetransfer.svg
--rw-r--r--   0        0        0    72424 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/additional-responses/image01.png
--rw-r--r--   0        0        0    70687 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/async-sql-databases/image01.png
--rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/behind-a-proxy/image01.png
--rw-r--r--   0        0        0    62026 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/behind-a-proxy/image02.png
--rw-r--r--   0        0        0    74280 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/behind-a-proxy/image03.png
--rw-r--r--   0        0        0    74516 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/bigger-applications/image01.png
--rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/bigger-applications/package.drawio
--rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/bigger-applications/package.svg
--rw-r--r--   0        0        0    55506 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/body/image01.png
--rw-r--r--   0        0        0    81208 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/body/image02.png
--rw-r--r--   0        0        0    66011 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/body/image03.png
--rw-r--r--   0        0        0    40151 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/body/image04.png
--rw-r--r--   0        0        0    52951 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/body/image05.png
--rw-r--r--   0        0        0    78746 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/body-fields/image01.png
--rw-r--r--   0        0        0    93828 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/body-fields/image02.png
--rw-r--r--   0        0        0    40992 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/body-nested-models/image01.png
--rw-r--r--   0        0        0    54866 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/custom-response/image01.png
--rw-r--r--   0        0        0    72574 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/dataclasses/image01.png
--rw-r--r--   0        0        0   173614 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/debugging/image01.png
--rw-r--r--   0        0        0    99443 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/debugging/image02.png
--rw-r--r--   0        0        0    79658 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/dependencies/image01.png
--rw-r--r--   0        0        0    66817 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/dependencies/image02.png
--rw-r--r--   0        0        0    64786 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/extending-openapi/image01.png
--rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/extending-openapi/image02.png
--rw-r--r--   0        0        0    11176 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/extending-openapi/image03.png
--rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/extending-openapi/image04.png
--rw-r--r--   0        0        0    78022 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/generate-clients/image01.png
--rw-r--r--   0        0        0    59828 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/generate-clients/image02.png
--rw-r--r--   0        0        0    61043 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/generate-clients/image03.png
--rw-r--r--   0        0        0    53853 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/generate-clients/image04.png
--rw-r--r--   0        0        0    31091 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/generate-clients/image05.png
--rw-r--r--   0        0        0    43434 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/generate-clients/image06.png
--rw-r--r--   0        0        0    49947 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/generate-clients/image07.png
--rw-r--r--   0        0        0    30019 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/generate-clients/image08.png
--rw-r--r--   0        0        0    95541 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/graphql/image01.png
--rw-r--r--   0        0        0    86437 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/metadata/image01.png
--rw-r--r--   0        0        0    47719 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/metadata/image02.png
--rw-r--r--   0        0        0    99295 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/openapi-callbacks/image01.png
--rw-r--r--   0        0        0    86925 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/openapi-webhooks/image01.png
--rw-r--r--   0        0        0    68080 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/path-operation-advanced-configuration/image01.png
--rw-r--r--   0        0        0    41919 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/path-operation-configuration/image01.png
--rw-r--r--   0        0        0    86975 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/path-operation-configuration/image02.png
--rw-r--r--   0        0        0    71050 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/path-operation-configuration/image03.png
--rw-r--r--   0        0        0    38687 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/path-operation-configuration/image04.png
--rw-r--r--   0        0        0    74423 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/path-operation-configuration/image05.png
--rw-r--r--   0        0        0    79109 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/path-params/image01.png
--rw-r--r--   0        0        0    67289 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/path-params/image02.png
--rw-r--r--   0        0        0   118540 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/path-params/image03.png
--rw-r--r--   0        0        0    86345 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/query-params-str-validations/image01.png
--rw-r--r--   0        0        0    72770 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/query-params-str-validations/image02.png
--rw-r--r--   0        0        0    76191 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/response-model/image01.png
--rw-r--r--   0        0        0    89115 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/response-model/image02.png
--rw-r--r--   0        0        0    74275 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/response-status-code/image01.png
--rw-r--r--   0        0        0    30455 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/response-status-code/image02.png
--rw-r--r--   0        0        0    53959 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/security/image01.png
--rw-r--r--   0        0        0    90212 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/security/image02.png
--rw-r--r--   0        0        0    92466 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/security/image03.png
--rw-r--r--   0        0        0    84481 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/security/image04.png
--rw-r--r--   0        0        0    81962 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/security/image05.png
--rw-r--r--   0        0        0    91545 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/security/image06.png
--rw-r--r--   0        0        0    61135 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/security/image07.png
--rw-r--r--   0        0        0    88705 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/security/image08.png
--rw-r--r--   0        0        0   110760 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/security/image09.png
--rw-r--r--   0        0        0   159081 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/security/image10.png
--rw-r--r--   0        0        0    77654 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/security/image11.png
--rw-r--r--   0        0        0    69280 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/security/image12.png
--rw-r--r--   0        0        0    78949 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/sql-databases/image01.png
--rw-r--r--   0        0        0    83482 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/sql-databases/image02.png
--rw-r--r--   0        0        0    50472 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/sub-applications/image01.png
--rw-r--r--   0        0        0    53366 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/sub-applications/image02.png
--rw-r--r--   0        0        0    17229 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/websockets/image01.png
--rw-r--r--   0        0        0    18326 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/websockets/image02.png
--rw-r--r--   0        0        0    21283 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/websockets/image03.png
--rw-r--r--   0        0        0    30900 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/websockets/image04.png
--rw-r--r--   0        0        0    53330 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/img/tutorial/websockets/image05.png
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/js/chat.js
--rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/js/termynal.js
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/background-tasks.md
--rw-r--r--   0        0        0    18654 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/bigger-applications.md
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/body-fields.md
--rw-r--r--   0        0        0     7858 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/body-multiple-params.md
--rw-r--r--   0        0        0     9735 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/body-nested-models.md
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/body-updates.md
--rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/body.md
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/cookie-params.md
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/cors.md
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/debugging.md
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/encoder.md
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/extra-data-types.md
--rw-r--r--   0        0        0     7567 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/extra-models.md
--rw-r--r--   0        0        0     9445 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/handling-errors.md
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/header-params.md
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/index.md
--rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/metadata.md
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/middleware.md
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/path-operation-configuration.md
--rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/path-params-numeric-validations.md
--rw-r--r--   0        0        0     9279 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/path-params.md
--rw-r--r--   0        0        0    26453 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/query-params-str-validations.md
--rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/query-params.md
--rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/request-files.md
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/request-forms-and-files.md
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/request-forms.md
--rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/response-model.md
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/response-status-code.md
--rw-r--r--   0        0        0     8589 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/schema-extra-example.md
--rw-r--r--   0        0        0    29642 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/sql-databases.md
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/static-files.md
--rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/testing.md
--rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/dependencies/classes-as-dependencies.md
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md
--rw-r--r--   0        0        0    10848 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/dependencies/dependencies-with-yield.md
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/dependencies/global-dependencies.md
--rw-r--r--   0        0        0    11857 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/dependencies/index.md
--rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/dependencies/sub-dependencies.md
--rw-r--r--   0        0        0     9112 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/security/first-steps.md
--rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/security/get-current-user.md
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/security/index.md
--rw-r--r--   0        0        0    13286 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/security/oauth2-jwt.md
--rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/docs/tutorial/security/simple-oauth2.md
--rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/layouts/custom.yml
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/en/overrides/main.html
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/es/mkdocs.yml
--rw-r--r--   0        0        0    25513 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/es/docs/async.md
--rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/es/docs/features.md
--rw-r--r--   0        0        0    19381 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/es/docs/index.md
--rw-r--r--   0        0        0     9390 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/es/docs/python-types.md
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/es/docs/advanced/additional-status-codes.md
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/es/docs/advanced/index.md
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/es/docs/advanced/path-operation-advanced-configuration.md
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/es/docs/advanced/response-directly.md
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/es/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/es/docs/tutorial/index.md
--rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/es/docs/tutorial/path-params.md
--rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/es/docs/tutorial/query-params.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fa/mkdocs.yml
--rw-r--r--   0        0        0    26471 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fa/docs/index.md
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fa/docs/advanced/sub-applications.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/mkdocs.yml
--rw-r--r--   0        0        0    28159 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/alternatives.md
--rw-r--r--   0        0        0    24572 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/async.md
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/external-links.md
--rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/fastapi-people.md
--rw-r--r--   0        0        0    11587 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/features.md
--rw-r--r--   0        0        0     7339 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/help-fastapi.md
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/history-design-future.md
--rw-r--r--   0        0        0    22510 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/index.md
--rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/project-generation.md
--rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/python-types.md
--rw-r--r--   0        0        0     9841 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/advanced/additional-responses.md
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/advanced/additional-status-codes.md
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/advanced/index.md
--rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/advanced/path-operation-advanced-configuration.md
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/advanced/response-directly.md
--rw-r--r--   0        0        0     6356 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/deployment/deta.md
--rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/deployment/docker.md
--rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/deployment/https.md
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/deployment/index.md
--rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/deployment/manually.md
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/deployment/versions.md
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/tutorial/background-tasks.md
--rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/tutorial/body.md
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/tutorial/debugging.md
--rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/tutorial/path-params.md
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/fr/docs/tutorial/query-params.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/he/mkdocs.yml
--rw-r--r--   0        0        0    21642 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/he/docs/index.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/id/mkdocs.yml
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/id/docs/tutorial/index.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/mkdocs.yml
--rw-r--r--   0        0        0    32353 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/alternatives.md
--rw-r--r--   0        0        0    28468 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/async.md
--rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/benchmarks.md
--rw-r--r--   0        0        0    17028 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/contributing.md
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/external-links.md
--rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/fastapi-people.md
--rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/features.md
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/help-fastapi.md
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/history-design-future.md
--rw-r--r--   0        0        0    21414 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/index.md
--rw-r--r--   0        0        0     7264 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/project-generation.md
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/advanced/additional-status-codes.md
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/advanced/conditional-openapi.md
--rw-r--r--   0        0        0    10906 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/advanced/custom-response.md
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/advanced/index.md
--rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/advanced/nosql-databases.md
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/advanced/path-operation-advanced-configuration.md
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/advanced/response-directly.md
--rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/advanced/websockets.md
--rw-r--r--   0        0        0     6667 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/deployment/deta.md
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/deployment/docker.md
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/deployment/index.md
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/deployment/manually.md
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/deployment/versions.md
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/tutorial/body-updates.md
--rw-r--r--   0        0        0     8130 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/tutorial/body.md
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/tutorial/cookie-params.md
--rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/tutorial/cors.md
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/tutorial/debugging.md
--rw-r--r--   0        0        0    11456 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/tutorial/header-params.md
--rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/tutorial/index.md
--rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/tutorial/middleware.md
--rw-r--r--   0        0        0    10867 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/tutorial/path-params.md
--rw-r--r--   0        0        0    10789 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/tutorial/query-params-str-validations.md
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/tutorial/query-params.md
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/tutorial/request-forms.md
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/tutorial/static-files.md
--rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/tutorial/testing.md
--rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/tutorial/security/first-steps.md
--rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ja/docs/tutorial/security/oauth2-jwt.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ko/mkdocs.yml
--rw-r--r--   0        0        0    19874 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ko/docs/index.md
--rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ko/docs/deployment/versions.md
--rw-r--r--   0        0        0     5905 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ko/docs/tutorial/cors.md
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ko/docs/tutorial/encoder.md
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ko/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ko/docs/tutorial/header-params.md
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ko/docs/tutorial/index.md
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ko/docs/tutorial/path-params-numeric-validations.md
--rw-r--r--   0        0        0     9880 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ko/docs/tutorial/path-params.md
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ko/docs/tutorial/query-params.md
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ko/docs/tutorial/request-files.md
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ko/docs/tutorial/request-forms-and-files.md
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ko/docs/tutorial/response-status-code.md
--rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ko/docs/tutorial/dependencies/classes-as-dependencies.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pl/mkdocs.yml
--rw-r--r--   0        0        0    11372 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pl/docs/features.md
--rw-r--r--   0        0        0    19762 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pl/docs/index.md
--rw-r--r--   0        0        0    10055 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pl/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pl/docs/tutorial/index.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/mkdocs.yml
--rw-r--r--   0        0        0    26158 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/alternatives.md
--rw-r--r--   0        0        0    22758 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/async.md
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/benchmarks.md
--rw-r--r--   0        0        0    15229 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/contributing.md
--rw-r--r--   0        0        0    17171 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/deployment.md
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/external-links.md
--rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/fastapi-people.md
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/features.md
--rw-r--r--   0        0        0     8848 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/help-fastapi.md
--rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/history-design-future.md
--rw-r--r--   0        0        0    19034 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/index.md
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/project-generation.md
--rw-r--r--   0        0        0     9892 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/python-types.md
--rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/advanced/events.md
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/advanced/index.md
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/deployment/deta.md
--rw-r--r--   0        0        0    38309 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/deployment/docker.md
--rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/deployment/https.md
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/deployment/index.md
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/deployment/versions.md
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/background-tasks.md
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/body-fields.md
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/body-multiple-params.md
--rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/body-nested-models.md
--rw-r--r--   0        0        0     7294 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/body.md
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/cookie-params.md
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/encoder.md
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/extra-data-types.md
--rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/extra-models.md
--rw-r--r--   0        0        0     9849 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0    10274 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/handling-errors.md
--rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/header-params.md
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/index.md
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/path-operation-configuration.md
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/path-params-numeric-validations.md
--rw-r--r--   0        0        0     9946 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/path-params.md
--rw-r--r--   0        0        0     9547 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/query-params-str-validations.md
--rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/query-params.md
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/request-forms-and-files.md
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/request-forms.md
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/response-status-code.md
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/static-files.md
--rw-r--r--   0        0        0     8499 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/security/first-steps.md
--rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/pt/docs/tutorial/security/index.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/mkdocs.yml
--rw-r--r--   0        0        0    40311 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/alternatives.md
--rw-r--r--   0        0        0    40878 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/async.md
--rw-r--r--   0        0        0     6201 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/benchmarks.md
--rw-r--r--   0        0        0    23066 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/contributing.md
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/external-links.md
--rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/fastapi-people.md
--rw-r--r--   0        0        0    16914 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/features.md
--rw-r--r--   0        0        0    23415 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/help-fastapi.md
--rw-r--r--   0        0        0     7421 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/history-design-future.md
--rw-r--r--   0        0        0    26377 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/index.md
--rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/project-generation.md
--rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/python-types.md
--rw-r--r--   0        0        0    33259 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/deployment/concepts.md
--rw-r--r--   0        0        0    21137 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/deployment/https.md
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/deployment/index.md
--rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/deployment/manually.md
--rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/deployment/versions.md
--rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/background-tasks.md
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/body-fields.md
--rw-r--r--   0        0        0    11923 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/body-multiple-params.md
--rw-r--r--   0        0        0    15297 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/body-nested-models.md
--rw-r--r--   0        0        0    11229 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/body.md
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/cookie-params.md
--rw-r--r--   0        0        0     8540 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/cors.md
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/debugging.md
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/extra-data-types.md
--rw-r--r--   0        0        0    11832 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/extra-models.md
--rw-r--r--   0        0        0    13423 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/index.md
--rw-r--r--   0        0        0     8533 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/metadata.md
--rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/path-operation-configuration.md
--rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/path-params-numeric-validations.md
--rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/path-params.md
--rw-r--r--   0        0        0    38884 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/query-params-str-validations.md
--rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/query-params.md
--rw-r--r--   0        0        0    31261 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/response-model.md
--rw-r--r--   0        0        0     7166 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/response-status-code.md
--rw-r--r--   0        0        0    11861 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/schema-extra-example.md
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/static-files.md
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/ru/docs/tutorial/testing.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/tr/mkdocs.yml
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/tr/docs/benchmarks.md
--rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/tr/docs/fastapi-people.md
--rw-r--r--   0        0        0    11579 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/tr/docs/features.md
--rw-r--r--   0        0        0    20543 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/tr/docs/index.md
--rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/tr/docs/python-types.md
--rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/tr/docs/tutorial/first_steps.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/mkdocs.yml
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/benchmarks.md
--rw-r--r--   0        0        0    13647 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/contributing.md
--rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/fastapi-people.md
--rw-r--r--   0        0        0     9335 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/features.md
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/help-fastapi.md
--rw-r--r--   0        0        0    18357 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/index.md
--rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/python-types.md
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/advanced/additional-status-codes.md
--rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/advanced/custom-response.md
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/advanced/index.md
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/advanced/path-operation-advanced-configuration.md
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/advanced/response-change-status-code.md
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/advanced/response-cookies.md
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/advanced/response-directly.md
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/advanced/response-headers.md
--rw-r--r--   0        0        0    14283 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/advanced/settings.md
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/advanced/websockets.md
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/advanced/wsgi.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/advanced/security/index.md
--rw-r--r--   0        0        0    18647 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/bigger-applications.md
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/body-fields.md
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/body-multiple-params.md
--rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/body-nested-models.md
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/body-updates.md
--rw-r--r--   0        0        0     5620 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/body.md
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/cookie-params.md
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/cors.md
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/debugging.md
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/encoder.md
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/extra-data-types.md
--rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/extra-models.md
--rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/handling-errors.md
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/header-params.md
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/index.md
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/metadata.md
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/middleware.md
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/path-operation-configuration.md
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/path-params-numeric-validations.md
--rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/path-params.md
--rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/query-params-str-validations.md
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/query-params.md
--rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/request-files.md
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/request-forms-and-files.md
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/request-forms.md
--rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/response-model.md
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/response-status-code.md
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/schema-extra-example.md
--rw-r--r--   0        0        0    27546 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/sql-databases.md
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/static-files.md
--rw-r--r--   0        0        0     6107 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/testing.md
--rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/dependencies/classes-as-dependencies.md
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/dependencies/global-dependencies.md
--rw-r--r--   0        0        0     7190 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/dependencies/index.md
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/dependencies/sub-dependencies.md
--rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/security/first-steps.md
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/security/get-current-user.md
--rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/security/index.md
--rw-r--r--   0        0        0     9457 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/security/oauth2-jwt.md
--rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs/zh/docs/tutorial/security/simple-oauth2.md
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/additional_responses/tutorial001.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/additional_responses/tutorial002.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/additional_responses/tutorial003.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/additional_responses/tutorial004.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/additional_status_codes/tutorial001.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/additional_status_codes/tutorial001_an.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/additional_status_codes/tutorial001_an_py310.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/additional_status_codes/tutorial001_an_py39.py
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/additional_status_codes/tutorial001_py310.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/advanced_middleware/tutorial001.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/advanced_middleware/tutorial002.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/advanced_middleware/tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/main.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/test_main.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/tutorial001.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/tutorial002.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/app_b/__init__.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/app_b/main.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/app_b/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/app_b_an/__init__.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/app_b_an/main.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/app_b_an/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/app_b_an_py310/__init__.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/app_b_an_py310/main.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/app_b_an_py310/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/app_b_an_py39/__init__.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/app_b_an_py39/main.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/app_b_an_py39/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/app_b_py310/__init__.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/app_b_py310/main.py
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/app_testing/app_b_py310/test_main.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/async_sql_databases/tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/async_tests/__init__.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/async_tests/main.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/async_tests/test_main.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/background_tasks/tutorial001.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/background_tasks/tutorial002.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/background_tasks/tutorial002_an.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/background_tasks/tutorial002_an_py310.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/background_tasks/tutorial002_an_py39.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/background_tasks/tutorial002_py310.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/behind_a_proxy/tutorial001.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/behind_a_proxy/tutorial002.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/behind_a_proxy/tutorial003.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/behind_a_proxy/tutorial004.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app/dependencies.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app/internal/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app/internal/admin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app/routers/__init__.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app/routers/items.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app/routers/users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app_an/__init__.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app_an/dependencies.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app_an/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app_an/internal/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app_an/internal/admin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app_an/routers/__init__.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app_an/routers/items.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app_an/routers/users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app_an_py39/__init__.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app_an_py39/dependencies.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app_an_py39/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app_an_py39/internal/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app_an_py39/internal/admin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app_an_py39/routers/__init__.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app_an_py39/routers/items.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/bigger_applications/app_an_py39/routers/users.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body/tutorial001.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body/tutorial001_py310.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body/tutorial002.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body/tutorial002_py310.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body/tutorial003.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body/tutorial003_py310.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body/tutorial004.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body/tutorial004_py310.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_fields/tutorial001.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_fields/tutorial001_an.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_fields/tutorial001_an_py310.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_fields/tutorial001_an_py39.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_fields/tutorial001_py310.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial001.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial001_an.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial001_an_py310.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial001_an_py39.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial001_py310.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial002.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial002_py310.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial003.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial003_an.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial003_an_py310.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial003_an_py39.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial003_py310.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial004.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial004_an.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial004_an_py310.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial004_an_py39.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial004_py310.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial005.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial005_an.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial005_an_py310.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial005_an_py39.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_multiple_params/tutorial005_py310.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial001.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial001_py310.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial002.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial002_py310.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial002_py39.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial003.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial003_py310.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial003_py39.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial004.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial004_py310.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial004_py39.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial005.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial005_py310.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial005_py39.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial006.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial006_py310.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial006_py39.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial007.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial007_py310.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial007_py39.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial008.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial008_py39.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial009.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_nested_models/tutorial009_py39.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_updates/tutorial001.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_updates/tutorial001_py310.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_updates/tutorial001_py39.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_updates/tutorial002.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_updates/tutorial002_py310.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/body_updates/tutorial002_py39.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/conditional_openapi/tutorial001.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/cookie_params/tutorial001.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/cookie_params/tutorial001_an.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/cookie_params/tutorial001_an_py310.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/cookie_params/tutorial001_an_py39.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/cookie_params/tutorial001_py310.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/cors/tutorial001.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/custom_request_and_route/tutorial001.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/custom_request_and_route/tutorial002.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/custom_request_and_route/tutorial003.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/custom_response/tutorial001.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/custom_response/tutorial001b.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/custom_response/tutorial002.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/custom_response/tutorial003.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/custom_response/tutorial004.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/custom_response/tutorial005.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/custom_response/tutorial006.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/custom_response/tutorial006b.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/custom_response/tutorial006c.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/custom_response/tutorial007.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/custom_response/tutorial008.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/custom_response/tutorial009.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/custom_response/tutorial009b.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/custom_response/tutorial009c.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/custom_response/tutorial010.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dataclasses/tutorial001.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dataclasses/tutorial002.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dataclasses/tutorial003.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/debugging/tutorial001.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial001.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial001_02_an.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial001_02_an_py310.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial001_02_an_py39.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial001_an.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial001_an_py310.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial001_an_py39.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial001_py310.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial002.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial002_an.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial002_an_py310.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial002_an_py39.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial002_py310.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial003.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial003_an.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial003_an_py310.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial003_an_py39.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial003_py310.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial004.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial004_an.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial004_an_py310.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial004_an_py39.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial004_py310.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial005.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial005_an.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial005_an_py310.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial005_an_py39.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial005_py310.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial006.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial006_an.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial006_an_py39.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial007.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial008.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial008_an.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial008_an_py39.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial009.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial010.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial011.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial011_an.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial011_an_py39.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial012.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial012_an.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependencies/tutorial012_an_py39.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependency_testing/tutorial001.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependency_testing/tutorial001_an.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependency_testing/tutorial001_an_py310.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependency_testing/tutorial001_an_py39.py
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/dependency_testing/tutorial001_py310.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/encoder/tutorial001.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/encoder/tutorial001_py310.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/events/tutorial001.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/events/tutorial002.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/events/tutorial003.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extending_openapi/tutorial001.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extending_openapi/tutorial002.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extending_openapi/tutorial003.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extending_openapi/tutorial004.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extending_openapi/tutorial005.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extra_data_types/tutorial001.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extra_data_types/tutorial001_an.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extra_data_types/tutorial001_an_py310.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extra_data_types/tutorial001_an_py39.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extra_data_types/tutorial001_py310.py
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extra_models/tutorial001.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extra_models/tutorial001_py310.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extra_models/tutorial002.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extra_models/tutorial002_py310.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extra_models/tutorial003.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extra_models/tutorial003_py310.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extra_models/tutorial004.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extra_models/tutorial004_py39.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extra_models/tutorial005.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/extra_models/tutorial005_py39.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/first_steps/tutorial001.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/first_steps/tutorial002.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/first_steps/tutorial003.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/generate_clients/tutorial001.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/generate_clients/tutorial001_py39.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/generate_clients/tutorial002.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/generate_clients/tutorial002_py39.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/generate_clients/tutorial003.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/generate_clients/tutorial003_py39.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/generate_clients/tutorial004.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/graphql/tutorial001.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/handling_errors/tutorial001.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/handling_errors/tutorial002.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/handling_errors/tutorial003.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/handling_errors/tutorial004.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/handling_errors/tutorial005.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/handling_errors/tutorial006.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/header_params/tutorial001.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/header_params/tutorial001_an.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/header_params/tutorial001_an_py310.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/header_params/tutorial001_an_py39.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/header_params/tutorial001_py310.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/header_params/tutorial002.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/header_params/tutorial002_an.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/header_params/tutorial002_an_py310.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/header_params/tutorial002_an_py39.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/header_params/tutorial002_py310.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/header_params/tutorial003.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/header_params/tutorial003_an.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/header_params/tutorial003_an_py310.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/header_params/tutorial003_an_py39.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/header_params/tutorial003_py310.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/header_params/tutorial003_py39.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/metadata/tutorial001.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/metadata/tutorial001_1.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/metadata/tutorial002.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/metadata/tutorial003.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/metadata/tutorial004.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/middleware/tutorial001.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/nosql_databases/tutorial001.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/openapi_callbacks/tutorial001.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/openapi_webhooks/tutorial001.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_advanced_configuration/tutorial001.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_advanced_configuration/tutorial002.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_advanced_configuration/tutorial003.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_advanced_configuration/tutorial004.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_advanced_configuration/tutorial005.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_advanced_configuration/tutorial006.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_advanced_configuration/tutorial007.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_configuration/tutorial001.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_configuration/tutorial001_py310.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_configuration/tutorial001_py39.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_configuration/tutorial002.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_configuration/tutorial002_py310.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_configuration/tutorial002_py39.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_configuration/tutorial002b.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_configuration/tutorial003.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_configuration/tutorial003_py310.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_configuration/tutorial003_py39.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_configuration/tutorial004.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_configuration/tutorial004_py310.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_configuration/tutorial004_py39.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_configuration/tutorial005.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_configuration/tutorial005_py310.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_configuration/tutorial005_py39.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_operation_configuration/tutorial006.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params/tutorial001.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params/tutorial002.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params/tutorial003.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params/tutorial003b.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params/tutorial004.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params/tutorial005.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial001.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial001_an.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial001_an_py310.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial001_an_py39.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial001_py310.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial002.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial002_an.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial002_an_py39.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial003.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial003_an.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial003_an_py39.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial004.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial004_an.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial004_an_py39.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial005.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial005_an.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial005_an_py39.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial006.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial006_an.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/path_params_numeric_validations/tutorial006_an_py39.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial001.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial002.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial003.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial004.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial005.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial006.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial006_py39.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial007.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial007_py39.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial008.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial008_py39.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial008b.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial008b_py310.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial009.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial009_py310.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial009b.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial009c.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial009c_py310.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial010.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial011.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial011_py310.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial011_py39.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial012.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial013.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/python_types/tutorial013_py39.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params/tutorial001.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params/tutorial002.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params/tutorial002_py310.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params/tutorial003.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params/tutorial003_py310.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params/tutorial004.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params/tutorial004_py310.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params/tutorial005.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params/tutorial006.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params/tutorial006_py310.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params/tutorial006b.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial001.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial001_py310.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial002.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial002_an.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial002_an_py310.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial002_py310.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial003.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial003_an.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial003_an_py310.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial003_an_py39.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial003_py310.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial004.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial004_an.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial004_an_py310.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial004_an_py39.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial004_py310.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial005.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial005_an.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial005_an_py39.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial006.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial006_an.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial006_an_py39.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial006b.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial006b_an.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial006b_an_py39.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial006c.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial006c_an.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial006c_an_py310.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial006c_an_py39.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial006c_py310.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial006d.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial006d_an.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial006d_an_py39.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial007.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial007_an.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial007_an_py310.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial007_an_py39.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial007_py310.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial008.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial008_an.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial008_an_py310.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial008_an_py39.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial008_py310.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial009.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial009_an.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial009_an_py310.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial009_an_py39.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial009_py310.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial010.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial010_an.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial010_an_py310.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial010_an_py39.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial010_py310.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial011.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial011_an.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial011_an_py310.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial011_an_py39.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial011_py310.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial011_py39.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial012.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial012_an.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial012_an_py39.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial012_py39.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial013.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial013_an.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial013_an_py39.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial014.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial014_an.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial014_an_py310.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial014_an_py39.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/query_params_str_validations/tutorial014_py310.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_files/tutorial001.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_files/tutorial001_02.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_files/tutorial001_02_an.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_files/tutorial001_02_an_py310.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_files/tutorial001_02_an_py39.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_files/tutorial001_02_py310.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_files/tutorial001_03.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_files/tutorial001_03_an.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_files/tutorial001_03_an_py39.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_files/tutorial001_an.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_files/tutorial001_an_py39.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_files/tutorial002.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_files/tutorial002_an.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_files/tutorial002_an_py39.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_files/tutorial002_py39.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_files/tutorial003.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_files/tutorial003_an.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_files/tutorial003_an_py39.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_files/tutorial003_py39.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_forms/tutorial001.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_forms/tutorial001_an.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_forms/tutorial001_an_py39.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_forms_and_files/tutorial001.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_forms_and_files/tutorial001_an.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/request_forms_and_files/tutorial001_an_py39.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_change_status_code/tutorial001.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_cookies/tutorial001.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_cookies/tutorial002.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_directly/tutorial001.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_directly/tutorial002.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_headers/tutorial001.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_headers/tutorial002.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial001.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial001_01.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial001_01_py310.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial001_01_py39.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial001_py310.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial001_py39.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial002.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial002_py310.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial003.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial003_01.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial003_01_py310.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial003_02.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial003_03.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial003_04.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial003_04_py310.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial003_05.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial003_05_py310.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial003_py310.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial004.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial004_py310.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial004_py39.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial005.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial005_py310.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial006.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_model/tutorial006_py310.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_status_code/tutorial001.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/response_status_code/tutorial002.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/schema_extra_example/tutorial001.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/schema_extra_example/tutorial001_py310.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/schema_extra_example/tutorial002.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/schema_extra_example/tutorial002_py310.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/schema_extra_example/tutorial003.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/schema_extra_example/tutorial003_an.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/schema_extra_example/tutorial003_an_py310.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/schema_extra_example/tutorial003_an_py39.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/schema_extra_example/tutorial003_py310.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/schema_extra_example/tutorial004.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/schema_extra_example/tutorial004_an.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/schema_extra_example/tutorial004_an_py310.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/schema_extra_example/tutorial004_an_py39.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/schema_extra_example/tutorial004_py310.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial001.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial001_an.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial001_an_py39.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial002.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial002_an.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial002_an_py310.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial002_an_py39.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial002_py310.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial003.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial003_an.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial003_an_py310.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial003_an_py39.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial003_py310.py
--rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial004.py
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial004_an.py
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial004_an_py310.py
--rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial004_an_py39.py
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial004_py310.py
--rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial005.py
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial005_an.py
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial005_an_py310.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial005_an_py39.py
--rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial005_py310.py
--rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial005_py39.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial006.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial006_an.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial006_an_py39.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial007.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial007_an.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/security/tutorial007_an_py39.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app01/__init__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app01/config.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app01/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app02/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app02/config.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app02/main.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app02/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app02_an/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app02_an/config.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app02_an/main.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app02_an/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app02_an_py39/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app02_an_py39/config.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app02_an_py39/main.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app02_an_py39/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app03/__init__.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app03/config.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app03/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app03_an/__init__.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app03_an/config.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app03_an/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app03_an_py39/__init__.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app03_an_py39/config.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/settings/app03_an_py39/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app/__init__.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app/alt_main.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app/crud.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app/database.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app/main.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app/models.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app/tests/__init__.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app/tests/test_sql_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app_py310/__init__.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app_py310/alt_main.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app_py310/crud.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app_py310/database.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app_py310/main.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app_py310/models.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app_py310/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app_py310/tests/__init__.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app_py39/__init__.py
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app_py39/alt_main.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app_py39/crud.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app_py39/database.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app_py39/main.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app_py39/models.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app_py39/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app_py39/tests/__init__.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases_peewee/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases_peewee/sql_app/__init__.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases_peewee/sql_app/crud.py
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases_peewee/sql_app/database.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases_peewee/sql_app/main.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases_peewee/sql_app/models.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sql_databases_peewee/sql_app/schemas.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/static_files/tutorial001.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/sub_applications/tutorial001.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/templates/tutorial001.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/templates/static/styles.css
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/templates/templates/item.html
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/using_request_directly/tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/websockets/__init__.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/websockets/tutorial001.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/websockets/tutorial002.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/websockets/tutorial002_an.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/websockets/tutorial002_an_py310.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/websockets/tutorial002_an_py39.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/websockets/tutorial002_py310.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/websockets/tutorial003.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/websockets/tutorial003_py39.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 fastapi-0.99.0/docs_src/wsgi/tutorial001.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/__init__.py
--rw-r--r--   0        0        0    40588 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/applications.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/background.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/concurrency.py
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/datastructures.py
--rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/encoders.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/exception_handlers.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/exceptions.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/logger.py
--rw-r--r--   0        0        0     8981 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/param_functions.py
--rw-r--r--   0        0        0    13207 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/py.typed
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/requests.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/responses.py
--rw-r--r--   0        0        0    56490 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/routing.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/staticfiles.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/templating.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/testclient.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/types.py
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/utils.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/websockets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/dependencies/__init__.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/dependencies/models.py
--rw-r--r--   0        0        0    30908 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/dependencies/utils.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/middleware/__init__.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/middleware/asyncexitstack.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/middleware/cors.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/middleware/gzip.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/middleware/httpsredirect.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/middleware/trustedhost.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/openapi/__init__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/openapi/constants.py
--rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/openapi/docs.py
--rw-r--r--   0        0        0    14447 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/openapi/models.py
--rw-r--r--   0        0        0    19576 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/openapi/utils.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/security/__init__.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/security/api_key.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/security/base.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/security/http.py
--rw-r--r--   0        0        0     8360 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/security/oauth2.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/security/open_id_connect_url.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 fastapi-0.99.0/fastapi/security/utils.py
--rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 fastapi-0.99.0/scripts/build-docs.sh
--rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 fastapi-0.99.0/scripts/clean.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 fastapi-0.99.0/scripts/docs-live.sh
--rw-r--r--   0        0        0     9995 2020-02-02 00:00:00.000000 fastapi-0.99.0/scripts/docs.py
--rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 fastapi-0.99.0/scripts/format.sh
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 fastapi-0.99.0/scripts/gitter_releases_bot.py
--rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 fastapi-0.99.0/scripts/lint.sh
--rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 fastapi-0.99.0/scripts/mkdocs_hooks.py
--rwxr-xr-x   0        0        0      337 2020-02-02 00:00:00.000000 fastapi-0.99.0/scripts/netlify-docs.sh
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 fastapi-0.99.0/scripts/notify.sh
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 fastapi-0.99.0/scripts/publish.sh
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 fastapi-0.99.0/scripts/test-cov-html.sh
--rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 fastapi-0.99.0/scripts/test.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/__init__.py
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/main.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_additional_properties.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_additional_response_extra.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_additional_responses_bad.py
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_additional_responses_custom_model_in_callback.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_additional_responses_custom_validationerror.py
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_additional_responses_default_validationerror.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_additional_responses_response_class.py
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_additional_responses_router.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_ambiguous_params.py
--rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_annotated.py
--rw-r--r--   0        0        0    49052 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_application.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_callable_endpoint.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_custom_middleware_exception.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_custom_route_class.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_custom_schema_fields.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_custom_swagger_ui_redirect.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_datastructures.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_datetime_custom_encoder.py
--rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_default_response_class.py
--rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_default_response_class_router.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_dependency_cache.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_dependency_class.py
--rw-r--r--   0        0        0    11269 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_dependency_contextmanager.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_dependency_contextvars.py
--rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_dependency_duplicates.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_dependency_normal_exceptions.py
--rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_dependency_overrides.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_dependency_security_overrides.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_deprecated_openapi_prefix.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_duplicate_models_openapi.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_empty_router.py
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_enforce_once_required_parameter.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_exception_handlers.py
--rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_extra_routes.py
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_filter_pydantic_sub_model.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_forms_from_non_typing_sequences.py
--rw-r--r--   0        0        0    68172 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_generate_unique_id_function.py
--rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_get_request_body.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_http_connection_injection.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_include_route.py
--rw-r--r--   0        0        0   367192 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_include_router_defaults_overrides.py
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_infer_param_optionality.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_inherited_custom_class.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_invalid_path_param.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_invalid_sequence_param.py
--rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_jsonable_encoder.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_local_docs.py
--rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_multi_body_errors.py
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_multi_query_errors.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_multipart_installation.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_no_swagger_ui_redirect.py
--rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_openapi_query_parameter_extension.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_openapi_route_extensions.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_openapi_servers.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_operations_signatures.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_orjson_response_class.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_param_class.py
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_param_in_path_and_dependency.py
--rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_param_include_in_schema.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_params_repr.py
--rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_path.py
--rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_put_no_body.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_query.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_read_with_orm_mode.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_repeated_cookie_headers.py
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_repeated_dependency_schema.py
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_repeated_parameter_alias.py
--rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_reponse_set_reponse_code_empty.py
--rw-r--r--   0        0        0     6546 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_request_body_parameters_media_type.py
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_required_noneable.py
--rw-r--r--   0        0        0    10951 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_response_by_alias.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_response_change_status_code.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_response_class_no_mediatype.py
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_response_code_no_body.py
--rw-r--r--   0        0        0    48457 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_response_model_as_return_annotation.py
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_response_model_include_exclude.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_response_model_invalid.py
--rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_response_model_sub_types.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_route_scope.py
--rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_router_events.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_router_prefix_with_template.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_router_redirect_slashes.py
--rw-r--r--   0        0        0    32406 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_schema_extra_examples.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_api_key_cookie.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_api_key_cookie_description.py
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_api_key_cookie_optional.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_api_key_header.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_api_key_header_description.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_api_key_header_optional.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_api_key_query.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_api_key_query_description.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_api_key_query_optional.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_http_base.py
--rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_http_base_description.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_http_base_optional.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_http_basic_optional.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_http_basic_realm.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_http_basic_realm_description.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_http_bearer.py
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_http_bearer_description.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_http_bearer_optional.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_http_digest.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_http_digest_description.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_http_digest_optional.py
--rw-r--r--   0        0        0     8340 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_oauth2.py
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_oauth2_authorization_code_bearer.py
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_oauth2_authorization_code_bearer_description.py
--rw-r--r--   0        0        0     8387 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_oauth2_optional.py
--rw-r--r--   0        0        0     8490 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_oauth2_optional_description.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_oauth2_password_bearer_optional.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_oauth2_password_bearer_optional_description.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_openid_connect.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_openid_connect_description.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_security_openid_connect_optional.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_serialize_response.py
--rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_serialize_response_dataclass.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_serialize_response_model.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_skip_defaults.py
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_starlette_exception.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_starlette_urlconvertors.py
--rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_sub_callbacks.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_swagger_ui_init_oauth.py
--rw-r--r--   0        0        0     9847 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tuples.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_typing_python39.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_union_body.py
--rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_union_inherited_body.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_validate_response.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_validate_response_dataclass.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_validate_response_recursive.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_webhooks_security.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_ws_dependencies.py
--rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_ws_router.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_modules_same_name_body/__init__.py
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_modules_same_name_body/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_modules_same_name_body/app/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_modules_same_name_body/app/a.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_modules_same_name_body/app/b.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_modules_same_name_body/app/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_additional_responses/__init__.py
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_additional_responses/test_tutorial001.py
--rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_additional_responses/test_tutorial002.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_additional_responses/test_tutorial003.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_additional_responses/test_tutorial004.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_additional_status_codes/__init__.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_advanced_middleware/__init__.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_advanced_middleware/test_tutorial001.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_async_sql_databases/__init__.py
--rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_async_tests/__init__.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_async_tests/test_main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_background_tasks/__init__.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_background_tasks/test_tutorial001.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_background_tasks/test_tutorial002.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_behind_a_proxy/__init__.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_bigger_applications/__init__.py
--rw-r--r--   0        0        0    18714 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_bigger_applications/test_main.py
--rw-r--r--   0        0        0    18717 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_bigger_applications/test_main_an.py
--rw-r--r--   0        0        0    19078 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body/__init__.py
--rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body/test_tutorial001.py
--rw-r--r--   0        0        0     9101 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_fields/__init__.py
--rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_fields/test_tutorial001.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_fields/test_tutorial001_an.py
--rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/__init__.py
--rw-r--r--   0        0        0     5239 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py
--rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py
--rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py
--rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py
--rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py
--rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py
--rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_nested_models/__init__.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_nested_models/test_tutorial009.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_updates/__init__.py
--rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_updates/test_tutorial001.py
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py
--rw-r--r--   0        0        0     6248 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_conditional_openapi/__init__.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_cookie_params/__init__.py
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_cookie_params/test_tutorial001.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_cors/__init__.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_cors/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_custom_request_and_route/__init__.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_custom_response/__init__.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_custom_response/test_tutorial001.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_custom_response/test_tutorial001b.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_custom_response/test_tutorial004.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_custom_response/test_tutorial005.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_custom_response/test_tutorial006.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_custom_response/test_tutorial006b.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_custom_response/test_tutorial006c.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_custom_response/test_tutorial007.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_custom_response/test_tutorial008.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_custom_response/test_tutorial009.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_custom_response/test_tutorial009b.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_custom_response/test_tutorial009c.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dataclasses/__init__.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dataclasses/test_tutorial001.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dataclasses/test_tutorial002.py
--rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dataclasses/test_tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dependencies/__init__.py
--rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial001.py
--rw-r--r--   0        0        0     6356 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial001_an.py
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py
--rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial004.py
--rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial004_an.py
--rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py
--rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial006.py
--rw-r--r--   0        0        0     4480 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial006_an.py
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py
--rw-r--r--   0        0        0     7386 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial012.py
--rw-r--r--   0        0        0     7389 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial012_an.py
--rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_events/__init__.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_events/test_tutorial001.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_events/test_tutorial002.py
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_events/test_tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_extending_openapi/__init__.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_extending_openapi/test_tutorial001.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_extending_openapi/test_tutorial002.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_extending_openapi/test_tutorial003.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_extending_openapi/test_tutorial004.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_extending_openapi/test_tutorial005.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_extra_data_types/__init__.py
--rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_extra_data_types/test_tutorial001.py
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py
--rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_extra_models/__init__.py
--rw-r--r--   0        0        0     4808 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_extra_models/test_tutorial003.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_extra_models/test_tutorial004.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_extra_models/test_tutorial005.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_first_steps/__init__.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_first_steps/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_generate_clients/__init__.py
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_generate_clients/test_tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_handling_errors/__init__.py
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_handling_errors/test_tutorial001.py
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_handling_errors/test_tutorial002.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_handling_errors/test_tutorial003.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_handling_errors/test_tutorial004.py
--rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_handling_errors/test_tutorial005.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_handling_errors/test_tutorial006.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_header_params/__init__.py
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial001.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial001_an.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial001_py310.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial002.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial002_an.py
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py
--rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial002_py310.py
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial003.py
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial003_an.py
--rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial003_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_metadata/__init__.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_metadata/test_tutorial001.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_metadata/test_tutorial001_1.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_metadata/test_tutorial004.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_openapi_callbacks/__init__.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_openapi_webhooks/__init__.py
--rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_openapi_webhooks/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_path_operation_advanced_configurations/__init__.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_path_operation_configurations/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py
--rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_path_params/__init__.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_path_params/test_tutorial004.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_path_params/test_tutorial005.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params/__init__.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params/test_tutorial005.py
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params/test_tutorial006.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params/test_tutorial006_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/__init__.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py
--rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/__init__.py
--rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001.py
--rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_02.py
--rw-r--r--   0        0        0     5987 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py
--rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py
--rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py
--rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_03.py
--rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py
--rw-r--r--   0        0        0     6300 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py
--rw-r--r--   0        0        0     6735 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_an.py
--rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     7703 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial002.py
--rw-r--r--   0        0        0     7706 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial002_an.py
--rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial002_py39.py
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial003.py
--rw-r--r--   0        0        0     7314 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial003_an.py
--rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     7827 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial003_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_forms/__init__.py
--rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_forms/test_tutorial001.py
--rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_forms/test_tutorial001_an.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_forms_and_files/__init__.py
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py
--rw-r--r--   0        0        0     6418 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py
--rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_change_status_code/__init__.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_cookies/__init__.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_cookies/test_tutorial001.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_cookies/test_tutorial002.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_headers/__init__.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_headers/test_tutorial001.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_headers/test_tutorial002.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_model/__init__.py
--rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial003.py
--rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial003_01.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py
--rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial003_02.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial003_03.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial003_04.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial003_04_py310.py
--rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial003_05.py
--rw-r--r--   0        0        0     3699 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py
--rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial003_py310.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial004.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial004_py310.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial004_py39.py
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial005.py
--rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial005_py310.py
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial006.py
--rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial006_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_schema_extra_example/__init__.py
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py
--rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py
--rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_security/__init__.py
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial001.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial001_an.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     6832 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial003.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial003_an.py
--rw-r--r--   0        0        0     7244 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial003_an_py310.py
--rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial003_an_py39.py
--rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial003_py310.py
--rw-r--r--   0        0        0    13084 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial005.py
--rw-r--r--   0        0        0    13087 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial005_an.py
--rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial005_an_py310.py
--rw-r--r--   0        0        0    13968 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial005_an_py39.py
--rw-r--r--   0        0        0    13980 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial005_py310.py
--rw-r--r--   0        0        0    13956 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial005_py39.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial006.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial006_an.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial006_an_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_settings/__init__.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_settings/test_app02.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_sql_databases/__init__.py
--rw-r--r--   0        0        0    15205 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_sql_databases/test_sql_databases.py
--rw-r--r--   0        0        0    15384 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py
--rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py
--rw-r--r--   0        0        0    15666 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py
--rw-r--r--   0        0        0    15681 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py
--rw-r--r--   0        0        0    15672 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_sql_databases/test_testing_databases.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_sql_databases_peewee/__init__.py
--rw-r--r--   0        0        0    17654 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_sql_databases_peewee/test_sql_databases_peewee.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_sub_applications/__init__.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_sub_applications/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_templates/__init__.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_templates/test_tutorial001.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_testing/__init__.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_testing/test_main.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_testing/test_main_b.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_testing/test_main_b_an.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_testing/test_main_b_an_py310.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_testing/test_main_b_an_py39.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_testing/test_main_b_py310.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_testing/test_tutorial001.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_testing/test_tutorial002.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_testing/test_tutorial003.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_testing_dependencies/__init__.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_websockets/__init__.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_websockets/test_tutorial001.py
--rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_websockets/test_tutorial002.py
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_websockets/test_tutorial002_an.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_websockets/test_tutorial002_py310.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_websockets/test_tutorial003.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_websockets/test_tutorial003_py39.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_wsgi/__init__.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastapi-0.99.0/tests/test_tutorial/test_wsgi/test_tutorial001.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 fastapi-0.99.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fastapi-0.99.0/LICENSE
--rw-r--r--   0        0        0    20581 2020-02-02 00:00:00.000000 fastapi-0.99.0/README.md
--rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 fastapi-0.99.0/pyproject.toml
--rw-r--r--   0        0        0    23001 2020-02-02 00:00:00.000000 fastapi-0.99.0/PKG-INFO
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fastapi-0.99.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi-0.99.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 fastapi-0.99.1/SECURITY.md
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 fastapi-0.99.1/requirements-docs.txt
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 fastapi-0.99.1/requirements-tests.txt
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 fastapi-0.99.1/requirements.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/DISCUSSION_TEMPLATE/questions.yml
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/ISSUE_TEMPLATE/privileged.yml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/actions/comment-docs-preview-in-pr/Dockerfile
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/actions/comment-docs-preview-in-pr/action.yml
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/actions/comment-docs-preview-in-pr/app/main.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/actions/notify-translations/Dockerfile
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/actions/notify-translations/action.yml
+-rw-r--r--   0        0        0    12661 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/actions/notify-translations/app/main.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/actions/people/Dockerfile
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/actions/people/action.yml
+-rw-r--r--   0        0        0    19794 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/actions/people/app/main.py
+-rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/workflows/build-docs.yml
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/workflows/deploy-docs.yml
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/workflows/issue-manager.yml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/workflows/label-approved.yml
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/workflows/notify-translations.yml
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/workflows/people.yml
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/workflows/smokeshow.yml
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 fastapi-0.99.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/missing-translation.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/de/mkdocs.yml
+-rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/de/docs/features.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/mkdocs.yml
+-rw-r--r--   0        0        0    19136 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/alternatives.md
+-rw-r--r--   0        0        0    19114 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/async.md
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/benchmarks.md
+-rw-r--r--   0        0        0    11702 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/contributing.md
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/external-links.md
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/fastapi-people.md
+-rw-r--r--   0        0        0     8409 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/features.md
+-rw-r--r--   0        0        0    12235 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/help-fastapi.md
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/history-design-future.md
+-rw-r--r--   0        0        0    17670 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/index.md
+-rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/project-generation.md
+-rw-r--r--   0        0        0    13966 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/python-types.md
+-rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/additional-responses.md
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/additional-status-codes.md
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/advanced-dependencies.md
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/async-sql-databases.md
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/async-tests.md
+-rw-r--r--   0        0        0    10306 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/behind-a-proxy.md
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/conditional-openapi.md
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/custom-request-and-route.md
+-rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/custom-response.md
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/dataclasses.md
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/events.md
+-rw-r--r--   0        0        0     9748 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/extending-openapi.md
+-rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/generate-clients.md
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/graphql.md
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/index.md
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/middleware.md
+-rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/nosql-databases.md
+-rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/openapi-callbacks.md
+-rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/path-operation-advanced-configuration.md
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/response-change-status-code.md
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/response-cookies.md
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/response-directly.md
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/response-headers.md
+-rw-r--r--   0        0        0    11642 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/settings.md
+-rw-r--r--   0        0        0    19705 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/sql-databases-peewee.md
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/sub-applications.md
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/templates.md
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/testing-database.md
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/testing-dependencies.md
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/testing-events.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/testing-websockets.md
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/using-request-directly.md
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/websockets.md
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/wsgi.md
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/security/http-basic-auth.md
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/security/index.md
+-rw-r--r--   0        0        0    11325 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/advanced/security/oauth2-scopes.md
+-rw-r--r--   0        0        0    14832 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/deployment/concepts.md
+-rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/deployment/deta.md
+-rw-r--r--   0        0        0    28740 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/deployment/docker.md
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/deployment/https.md
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/deployment/index.md
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/deployment/manually.md
+-rw-r--r--   0        0        0     8396 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/deployment/server-workers.md
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/deployment/versions.md
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/background-tasks.md
+-rw-r--r--   0        0        0    15678 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/bigger-applications.md
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/body-fields.md
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/body-multiple-params.md
+-rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/body-nested-models.md
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/body-updates.md
+-rw-r--r--   0        0        0     6683 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/body.md
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/cookie-params.md
+-rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/cors.md
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/debugging.md
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/encoder.md
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/extra-data-types.md
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/extra-models.md
+-rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/handling-errors.md
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/header-params.md
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/index.md
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/metadata.md
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/middleware.md
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/path-operation-configuration.md
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/path-params-numeric-validations.md
+-rw-r--r--   0        0        0     7878 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0    12188 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/query-params-str-validations.md
+-rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0     6803 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/request-files.md
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/request-forms-and-files.md
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/request-forms.md
+-rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/response-model.md
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/response-status-code.md
+-rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/schema-extra-example.md
+-rw-r--r--   0        0        0    25882 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/sql-databases.md
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/static-files.md
+-rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/testing.md
+-rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/dependencies/classes-as-dependencies.md
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md
+-rw-r--r--   0        0        0     8941 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/dependencies/dependencies-with-yield.md
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/dependencies/global-dependencies.md
+-rw-r--r--   0        0        0     6876 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/dependencies/index.md
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/dependencies/sub-dependencies.md
+-rw-r--r--   0        0        0     6946 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/security/first-steps.md
+-rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/security/get-current-user.md
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/security/index.md
+-rw-r--r--   0        0        0     9718 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/security/oauth2-jwt.md
+-rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/em/docs/tutorial/security/simple-oauth2.md
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/mkdocs.insiders.yml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/mkdocs.maybe-insiders.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/mkdocs.no-insiders.yml
+-rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/mkdocs.yml
+-rw-r--r--   0        0        0    19084 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/data/external_links.yml
+-rw-r--r--   0        0        0    25966 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/data/github_sponsors.yml
+-rw-r--r--   0        0        0    22157 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/data/people.yml
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/data/sponsors.yml
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/data/sponsors_badge.yml
+-rw-r--r--   0        0        0    23768 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/alternatives.md
+-rw-r--r--   0        0        0    23576 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/async.md
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/benchmarks.md
+-rw-r--r--   0        0        0    13506 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/contributing.md
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/external-links.md
+-rw-r--r--   0        0        0     6515 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/fastapi-people.md
+-rw-r--r--   0        0        0     9479 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/features.md
+-rw-r--r--   0        0        0    14258 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/help-fastapi.md
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/history-design-future.md
+-rw-r--r--   0        0        0    19216 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/index.md
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/newsletter.md
+-rw-r--r--   0        0        0     5826 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/project-generation.md
+-rw-r--r--   0        0        0    17461 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/python-types.md
+-rw-r--r--   0        0        0   278467 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/release-notes.md
+-rw-r--r--   0        0        0     8996 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/additional-responses.md
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/additional-status-codes.md
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/advanced-dependencies.md
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/async-sql-databases.md
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/async-tests.md
+-rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/behind-a-proxy.md
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/conditional-openapi.md
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/custom-request-and-route.md
+-rw-r--r--   0        0        0    11981 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/custom-response.md
+-rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/dataclasses.md
+-rw-r--r--   0        0        0     7828 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/events.md
+-rw-r--r--   0        0        0    11645 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/extending-openapi.md
+-rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/generate-clients.md
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/graphql.md
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/index.md
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/middleware.md
+-rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/nosql-databases.md
+-rw-r--r--   0        0        0     7934 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/openapi-callbacks.md
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/openapi-webhooks.md
+-rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/path-operation-advanced-configuration.md
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/response-change-status-code.md
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/response-cookies.md
+-rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/response-directly.md
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/response-headers.md
+-rw-r--r--   0        0        0    14584 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/settings.md
+-rw-r--r--   0        0        0    23622 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/sql-databases-peewee.md
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/sub-applications.md
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/templates.md
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/testing-database.md
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/testing-dependencies.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/testing-events.md
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/testing-websockets.md
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/using-request-directly.md
+-rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/websockets.md
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/wsgi.md
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/security/http-basic-auth.md
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/security/index.md
+-rw-r--r--   0        0        0    20945 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/advanced/security/oauth2-scopes.md
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/css/custom.css
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/css/termynal.css
+-rw-r--r--   0        0        0    18405 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/deployment/concepts.md
+-rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/deployment/deta.md
+-rw-r--r--   0        0        0    35157 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/deployment/docker.md
+-rw-r--r--   0        0        0    12240 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/deployment/https.md
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/deployment/index.md
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/deployment/manually.md
+-rw-r--r--   0        0        0     9364 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/deployment/server-workers.md
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/deployment/versions.md
+-rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/favicon.png
+-rw-r--r--   0        0        0    58136 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/github-social-preview.png
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/github-social-preview.svg
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/icon-transparent-bg.png
+-rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/icon-white-bg.png
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/icon-white.svg
+-rw-r--r--   0        0        0     7844 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/logo-teal-vector.svg
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/logo-teal.svg
+-rw-r--r--   0        0        0    51205 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/pycharm-completion.png
+-rw-r--r--   0        0        0    62417 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/vscode-completion.png
+-rw-r--r--   0        0        0   203390 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-01.png
+-rw-r--r--   0        0        0   166992 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-02.png
+-rw-r--r--   0        0        0   172943 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-03.png
+-rw-r--r--   0        0        0   163423 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-04.png
+-rw-r--r--   0        0        0   159869 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-05.png
+-rw-r--r--   0        0        0   164838 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-06.png
+-rw-r--r--   0        0        0   169968 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-07.png
+-rw-r--r--   0        0        0   225993 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-01.png
+-rw-r--r--   0        0        0   203644 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-02.png
+-rw-r--r--   0        0        0   168628 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-03.png
+-rw-r--r--   0        0        0   219429 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-04.png
+-rw-r--r--   0        0        0   185116 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-05.png
+-rw-r--r--   0        0        0   157113 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-06.png
+-rw-r--r--   0        0        0   124827 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/concepts/image01.png
+-rw-r--r--   0        0        0    10203 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/concepts/process-ram.drawio
+-rw-r--r--   0        0        0    16640 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/concepts/process-ram.svg
+-rw-r--r--   0        0        0    39996 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/deta/image01.png
+-rw-r--r--   0        0        0    48297 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/deta/image02.png
+-rw-r--r--   0        0        0    52704 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/deta/image03.png
+-rw-r--r--   0        0        0    49760 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/deta/image04.png
+-rw-r--r--   0        0        0    33130 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/deta/image05.png
+-rw-r--r--   0        0        0   105270 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/deta/image06.png
+-rw-r--r--   0        0        0    26363 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/https/https.drawio
+-rw-r--r--   0        0        0    40488 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/https/https.svg
+-rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/https/https01.drawio
+-rw-r--r--   0        0        0    10583 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/https/https01.svg
+-rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/https/https02.drawio
+-rw-r--r--   0        0        0    15794 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/https/https02.svg
+-rw-r--r--   0        0        0    12582 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/https/https03.drawio
+-rw-r--r--   0        0        0    21549 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/https/https03.svg
+-rw-r--r--   0        0        0    14291 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/https/https04.drawio
+-rw-r--r--   0        0        0    23265 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/https/https04.svg
+-rw-r--r--   0        0        0    15945 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/https/https05.drawio
+-rw-r--r--   0        0        0    26167 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/https/https05.svg
+-rw-r--r--   0        0        0    17470 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/https/https06.drawio
+-rw-r--r--   0        0        0    27919 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/https/https06.svg
+-rw-r--r--   0        0        0    19117 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/https/https07.drawio
+-rw-r--r--   0        0        0    29659 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/https/https07.svg
+-rw-r--r--   0        0        0    21427 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/https/https08.drawio
+-rw-r--r--   0        0        0    33876 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/deployment/https/https08.svg
+-rw-r--r--   0        0        0    74158 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/index/index-01-swagger-ui-simple.png
+-rw-r--r--   0        0        0    68468 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/index/index-02-redoc-simple.png
+-rw-r--r--   0        0        0    75099 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/index/index-03-swagger-02.png
+-rw-r--r--   0        0        0    67572 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/index/index-04-swagger-03.png
+-rw-r--r--   0        0        0    71441 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/index/index-05-swagger-04.png
+-rw-r--r--   0        0        0    78842 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/index/index-06-redoc-02.png
+-rw-r--r--   0        0        0     8036 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/logo-margin/logo-teal-vector.svg
+-rw-r--r--   0        0        0    17680 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/logo-margin/logo-teal.png
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/logo-margin/logo-teal.svg
+-rw-r--r--   0        0        0    21502 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/logo-margin/logo-white-bg.png
+-rw-r--r--   0        0        0    17722 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/python-types/image01.png
+-rw-r--r--   0        0        0    47799 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/python-types/image02.png
+-rw-r--r--   0        0        0    42872 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/python-types/image03.png
+-rw-r--r--   0        0        0    18604 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/python-types/image04.png
+-rw-r--r--   0        0        0    42637 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/python-types/image05.png
+-rw-r--r--   0        0        0    29581 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/python-types/image06.png
+-rw-r--r--   0        0        0    37057 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/budget-insight.svg
+-rw-r--r--   0        0        0    16949 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/calmcode.jpg
+-rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/classiq-banner.png
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/classiq.png
+-rw-r--r--   0        0        0   133690 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/cryptapi-banner.svg
+-rw-r--r--   0        0        0   111142 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/cryptapi.svg
+-rw-r--r--   0        0        0   122267 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/databento.svg
+-rw-r--r--   0        0        0    38162 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/deta-banner.svg
+-rw-r--r--   0        0        0    56518 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/deta.svg
+-rw-r--r--   0        0        0   110000 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/docarray-top-banner.svg
+-rw-r--r--   0        0        0   129629 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/docarray.svg
+-rw-r--r--   0        0        0    53417 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/doist-banner.svg
+-rw-r--r--   0        0        0    93166 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/doist.svg
+-rw-r--r--   0        0        0    21211 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/dropbase-banner.svg
+-rw-r--r--   0        0        0     7520 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/dropbase.svg
+-rw-r--r--   0        0        0    10556 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/exoflare.png
+-rw-r--r--   0        0        0    16235 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.png
+-rw-r--r--   0        0        0    34985 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.svg
+-rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/flint.png
+-rw-r--r--   0        0        0    31985 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/haystack-fastapi.svg
+-rw-r--r--   0        0        0   107893 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/imgwhale-banner.svg
+-rw-r--r--   0        0        0   108995 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/imgwhale.svg
+-rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/ines-course.jpg
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/investsuite.svg
+-rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/jina-ai-banner.png
+-rw-r--r--   0        0        0    26112 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/jina-ai.png
+-rw-r--r--   0        0        0    42239 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/jina-banner.svg
+-rw-r--r--   0        0        0   162873 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/jina-top-banner.svg
+-rw-r--r--   0        0        0   220435 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/jina.svg
+-rw-r--r--   0        0        0   108837 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/jina2.svg
+-rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/platform-sh-banner.png
+-rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/platform-sh.png
+-rw-r--r--   0        0        0    15311 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/powens.png
+-rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/striveworks-banner.png
+-rw-r--r--   0        0        0    22639 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/striveworks.png
+-rw-r--r--   0        0        0    34780 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/striveworks2.png
+-rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/svix.svg
+-rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/talkpython.png
+-rw-r--r--   0        0        0    26425 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/testdriven.svg
+-rw-r--r--   0        0        0    15198 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/vimso.png
+-rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/sponsors/wetransfer.svg
+-rw-r--r--   0        0        0    72424 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/additional-responses/image01.png
+-rw-r--r--   0        0        0    70687 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/async-sql-databases/image01.png
+-rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/behind-a-proxy/image01.png
+-rw-r--r--   0        0        0    62026 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/behind-a-proxy/image02.png
+-rw-r--r--   0        0        0    74280 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/behind-a-proxy/image03.png
+-rw-r--r--   0        0        0    74516 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/bigger-applications/image01.png
+-rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/bigger-applications/package.drawio
+-rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/bigger-applications/package.svg
+-rw-r--r--   0        0        0    55506 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/body/image01.png
+-rw-r--r--   0        0        0    81208 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/body/image02.png
+-rw-r--r--   0        0        0    66011 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/body/image03.png
+-rw-r--r--   0        0        0    40151 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/body/image04.png
+-rw-r--r--   0        0        0    52951 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/body/image05.png
+-rw-r--r--   0        0        0    78746 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/body-fields/image01.png
+-rw-r--r--   0        0        0    93828 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/body-fields/image02.png
+-rw-r--r--   0        0        0    40992 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/body-nested-models/image01.png
+-rw-r--r--   0        0        0    54866 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/custom-response/image01.png
+-rw-r--r--   0        0        0    72574 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/dataclasses/image01.png
+-rw-r--r--   0        0        0   173614 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/debugging/image01.png
+-rw-r--r--   0        0        0    99443 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/debugging/image02.png
+-rw-r--r--   0        0        0    79658 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/dependencies/image01.png
+-rw-r--r--   0        0        0    66817 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/dependencies/image02.png
+-rw-r--r--   0        0        0    64786 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/extending-openapi/image01.png
+-rw-r--r--   0        0        0    11292 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/extending-openapi/image02.png
+-rw-r--r--   0        0        0    11176 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/extending-openapi/image03.png
+-rw-r--r--   0        0        0    11180 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/extending-openapi/image04.png
+-rw-r--r--   0        0        0    78022 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/generate-clients/image01.png
+-rw-r--r--   0        0        0    59828 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/generate-clients/image02.png
+-rw-r--r--   0        0        0    61043 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/generate-clients/image03.png
+-rw-r--r--   0        0        0    53853 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/generate-clients/image04.png
+-rw-r--r--   0        0        0    31091 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/generate-clients/image05.png
+-rw-r--r--   0        0        0    43434 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/generate-clients/image06.png
+-rw-r--r--   0        0        0    49947 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/generate-clients/image07.png
+-rw-r--r--   0        0        0    30019 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/generate-clients/image08.png
+-rw-r--r--   0        0        0    95541 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/graphql/image01.png
+-rw-r--r--   0        0        0    86437 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/metadata/image01.png
+-rw-r--r--   0        0        0    47719 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/metadata/image02.png
+-rw-r--r--   0        0        0    99295 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/openapi-callbacks/image01.png
+-rw-r--r--   0        0        0    86925 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/openapi-webhooks/image01.png
+-rw-r--r--   0        0        0    68080 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/path-operation-advanced-configuration/image01.png
+-rw-r--r--   0        0        0    41919 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/path-operation-configuration/image01.png
+-rw-r--r--   0        0        0    86975 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/path-operation-configuration/image02.png
+-rw-r--r--   0        0        0    71050 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/path-operation-configuration/image03.png
+-rw-r--r--   0        0        0    38687 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/path-operation-configuration/image04.png
+-rw-r--r--   0        0        0    74423 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/path-operation-configuration/image05.png
+-rw-r--r--   0        0        0    79109 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/path-params/image01.png
+-rw-r--r--   0        0        0    67289 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/path-params/image02.png
+-rw-r--r--   0        0        0   118540 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/path-params/image03.png
+-rw-r--r--   0        0        0    86345 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/query-params-str-validations/image01.png
+-rw-r--r--   0        0        0    72770 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/query-params-str-validations/image02.png
+-rw-r--r--   0        0        0    76191 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/response-model/image01.png
+-rw-r--r--   0        0        0    89115 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/response-model/image02.png
+-rw-r--r--   0        0        0    74275 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/response-status-code/image01.png
+-rw-r--r--   0        0        0    30455 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/response-status-code/image02.png
+-rw-r--r--   0        0        0    53959 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/security/image01.png
+-rw-r--r--   0        0        0    90212 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/security/image02.png
+-rw-r--r--   0        0        0    92466 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/security/image03.png
+-rw-r--r--   0        0        0    84481 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/security/image04.png
+-rw-r--r--   0        0        0    81962 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/security/image05.png
+-rw-r--r--   0        0        0    91545 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/security/image06.png
+-rw-r--r--   0        0        0    61135 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/security/image07.png
+-rw-r--r--   0        0        0    88705 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/security/image08.png
+-rw-r--r--   0        0        0   110760 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/security/image09.png
+-rw-r--r--   0        0        0   159081 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/security/image10.png
+-rw-r--r--   0        0        0    77654 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/security/image11.png
+-rw-r--r--   0        0        0    69280 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/security/image12.png
+-rw-r--r--   0        0        0    78949 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/sql-databases/image01.png
+-rw-r--r--   0        0        0    83482 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/sql-databases/image02.png
+-rw-r--r--   0        0        0    50472 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/sub-applications/image01.png
+-rw-r--r--   0        0        0    53366 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/sub-applications/image02.png
+-rw-r--r--   0        0        0    17229 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/websockets/image01.png
+-rw-r--r--   0        0        0    18326 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/websockets/image02.png
+-rw-r--r--   0        0        0    21283 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/websockets/image03.png
+-rw-r--r--   0        0        0    30900 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/websockets/image04.png
+-rw-r--r--   0        0        0    53330 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/img/tutorial/websockets/image05.png
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/js/chat.js
+-rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/js/termynal.js
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/background-tasks.md
+-rw-r--r--   0        0        0    18654 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/bigger-applications.md
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/body-fields.md
+-rw-r--r--   0        0        0     7858 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/body-multiple-params.md
+-rw-r--r--   0        0        0     9735 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/body-nested-models.md
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/body-updates.md
+-rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/body.md
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/cookie-params.md
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/cors.md
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/debugging.md
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/encoder.md
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/extra-data-types.md
+-rw-r--r--   0        0        0     7567 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/extra-models.md
+-rw-r--r--   0        0        0     9445 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/handling-errors.md
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/header-params.md
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/index.md
+-rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/metadata.md
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/middleware.md
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/path-operation-configuration.md
+-rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/path-params-numeric-validations.md
+-rw-r--r--   0        0        0     9279 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0    26453 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/query-params-str-validations.md
+-rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/request-files.md
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/request-forms-and-files.md
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/request-forms.md
+-rw-r--r--   0        0        0    18046 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/response-model.md
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/response-status-code.md
+-rw-r--r--   0        0        0     8589 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/schema-extra-example.md
+-rw-r--r--   0        0        0    29642 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/sql-databases.md
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/static-files.md
+-rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/testing.md
+-rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/dependencies/classes-as-dependencies.md
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md
+-rw-r--r--   0        0        0    10848 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/dependencies/dependencies-with-yield.md
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/dependencies/global-dependencies.md
+-rw-r--r--   0        0        0    11857 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/dependencies/index.md
+-rw-r--r--   0        0        0     5742 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/dependencies/sub-dependencies.md
+-rw-r--r--   0        0        0     9112 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/security/first-steps.md
+-rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/security/get-current-user.md
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/security/index.md
+-rw-r--r--   0        0        0    13286 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/security/oauth2-jwt.md
+-rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/docs/tutorial/security/simple-oauth2.md
+-rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/layouts/custom.yml
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/en/overrides/main.html
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/es/mkdocs.yml
+-rw-r--r--   0        0        0    25513 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/es/docs/async.md
+-rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/es/docs/features.md
+-rw-r--r--   0        0        0    19381 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/es/docs/index.md
+-rw-r--r--   0        0        0     9390 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/es/docs/python-types.md
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/es/docs/advanced/additional-status-codes.md
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/es/docs/advanced/index.md
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/es/docs/advanced/path-operation-advanced-configuration.md
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/es/docs/advanced/response-directly.md
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/es/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/es/docs/tutorial/index.md
+-rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/es/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/es/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fa/mkdocs.yml
+-rw-r--r--   0        0        0    26471 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fa/docs/index.md
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fa/docs/advanced/sub-applications.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/mkdocs.yml
+-rw-r--r--   0        0        0    28159 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/alternatives.md
+-rw-r--r--   0        0        0    24572 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/async.md
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/external-links.md
+-rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/fastapi-people.md
+-rw-r--r--   0        0        0    11587 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/features.md
+-rw-r--r--   0        0        0     7339 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/help-fastapi.md
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/history-design-future.md
+-rw-r--r--   0        0        0    22510 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/index.md
+-rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/project-generation.md
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/python-types.md
+-rw-r--r--   0        0        0     9841 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/advanced/additional-responses.md
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/advanced/additional-status-codes.md
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/advanced/index.md
+-rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/advanced/path-operation-advanced-configuration.md
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/advanced/response-directly.md
+-rw-r--r--   0        0        0     6356 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/deployment/deta.md
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/deployment/docker.md
+-rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/deployment/https.md
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/deployment/index.md
+-rw-r--r--   0        0        0     5515 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/deployment/manually.md
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/deployment/versions.md
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/tutorial/background-tasks.md
+-rw-r--r--   0        0        0     7999 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/tutorial/body.md
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/tutorial/debugging.md
+-rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/fr/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/he/mkdocs.yml
+-rw-r--r--   0        0        0    21642 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/he/docs/index.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/id/mkdocs.yml
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/id/docs/tutorial/index.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/mkdocs.yml
+-rw-r--r--   0        0        0    32353 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/alternatives.md
+-rw-r--r--   0        0        0    28468 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/async.md
+-rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/benchmarks.md
+-rw-r--r--   0        0        0    17028 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/contributing.md
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/external-links.md
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/fastapi-people.md
+-rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/features.md
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/help-fastapi.md
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/history-design-future.md
+-rw-r--r--   0        0        0    21414 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/index.md
+-rw-r--r--   0        0        0     7264 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/project-generation.md
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/advanced/additional-status-codes.md
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/advanced/conditional-openapi.md
+-rw-r--r--   0        0        0    10906 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/advanced/custom-response.md
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/advanced/index.md
+-rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/advanced/nosql-databases.md
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/advanced/path-operation-advanced-configuration.md
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/advanced/response-directly.md
+-rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/advanced/websockets.md
+-rw-r--r--   0        0        0     6667 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/deployment/deta.md
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/deployment/docker.md
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/deployment/index.md
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/deployment/manually.md
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/deployment/versions.md
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/tutorial/body-updates.md
+-rw-r--r--   0        0        0     8130 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/tutorial/body.md
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/tutorial/cookie-params.md
+-rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/tutorial/cors.md
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/tutorial/debugging.md
+-rw-r--r--   0        0        0    11456 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/tutorial/header-params.md
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/tutorial/index.md
+-rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/tutorial/middleware.md
+-rw-r--r--   0        0        0    10867 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0    10789 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/tutorial/query-params-str-validations.md
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/tutorial/request-forms.md
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/tutorial/static-files.md
+-rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/tutorial/testing.md
+-rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/tutorial/security/first-steps.md
+-rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ja/docs/tutorial/security/oauth2-jwt.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ko/mkdocs.yml
+-rw-r--r--   0        0        0    19874 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ko/docs/index.md
+-rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ko/docs/deployment/versions.md
+-rw-r--r--   0        0        0     5905 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ko/docs/tutorial/cors.md
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ko/docs/tutorial/encoder.md
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ko/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ko/docs/tutorial/header-params.md
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ko/docs/tutorial/index.md
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ko/docs/tutorial/path-params-numeric-validations.md
+-rw-r--r--   0        0        0     9880 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ko/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ko/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ko/docs/tutorial/request-files.md
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ko/docs/tutorial/request-forms-and-files.md
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ko/docs/tutorial/response-status-code.md
+-rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ko/docs/tutorial/dependencies/classes-as-dependencies.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pl/mkdocs.yml
+-rw-r--r--   0        0        0    11372 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pl/docs/features.md
+-rw-r--r--   0        0        0    19762 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pl/docs/index.md
+-rw-r--r--   0        0        0    10055 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pl/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pl/docs/tutorial/index.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/mkdocs.yml
+-rw-r--r--   0        0        0    26158 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/alternatives.md
+-rw-r--r--   0        0        0    22758 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/async.md
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/benchmarks.md
+-rw-r--r--   0        0        0    15229 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/contributing.md
+-rw-r--r--   0        0        0    17171 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/deployment.md
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/external-links.md
+-rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/fastapi-people.md
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/features.md
+-rw-r--r--   0        0        0     8848 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/help-fastapi.md
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/history-design-future.md
+-rw-r--r--   0        0        0    19034 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/index.md
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/project-generation.md
+-rw-r--r--   0        0        0     9892 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/python-types.md
+-rw-r--r--   0        0        0     8854 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/advanced/events.md
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/advanced/index.md
+-rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/deployment/deta.md
+-rw-r--r--   0        0        0    38309 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/deployment/docker.md
+-rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/deployment/https.md
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/deployment/index.md
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/deployment/versions.md
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/background-tasks.md
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/body-fields.md
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/body-multiple-params.md
+-rw-r--r--   0        0        0     7563 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/body-nested-models.md
+-rw-r--r--   0        0        0     7294 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/body.md
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/cookie-params.md
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/encoder.md
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/extra-data-types.md
+-rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/extra-models.md
+-rw-r--r--   0        0        0     9849 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0    10274 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/handling-errors.md
+-rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/header-params.md
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/index.md
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/path-operation-configuration.md
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/path-params-numeric-validations.md
+-rw-r--r--   0        0        0     9946 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0     9547 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/query-params-str-validations.md
+-rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/request-forms-and-files.md
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/request-forms.md
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/response-status-code.md
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/static-files.md
+-rw-r--r--   0        0        0     8499 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/security/first-steps.md
+-rw-r--r--   0        0        0     4886 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/pt/docs/tutorial/security/index.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/mkdocs.yml
+-rw-r--r--   0        0        0    40311 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/alternatives.md
+-rw-r--r--   0        0        0    40878 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/async.md
+-rw-r--r--   0        0        0     6201 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/benchmarks.md
+-rw-r--r--   0        0        0    23066 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/contributing.md
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/external-links.md
+-rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/fastapi-people.md
+-rw-r--r--   0        0        0    16914 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/features.md
+-rw-r--r--   0        0        0    23415 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/help-fastapi.md
+-rw-r--r--   0        0        0     7421 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/history-design-future.md
+-rw-r--r--   0        0        0    26377 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/index.md
+-rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/project-generation.md
+-rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/python-types.md
+-rw-r--r--   0        0        0    33259 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/deployment/concepts.md
+-rw-r--r--   0        0        0    21137 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/deployment/https.md
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/deployment/index.md
+-rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/deployment/manually.md
+-rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/deployment/versions.md
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/background-tasks.md
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/body-fields.md
+-rw-r--r--   0        0        0    11923 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/body-multiple-params.md
+-rw-r--r--   0        0        0    15297 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/body-nested-models.md
+-rw-r--r--   0        0        0    11229 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/body.md
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/cookie-params.md
+-rw-r--r--   0        0        0     8540 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/cors.md
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/debugging.md
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/extra-data-types.md
+-rw-r--r--   0        0        0    11832 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/extra-models.md
+-rw-r--r--   0        0        0    13423 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     4825 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/index.md
+-rw-r--r--   0        0        0     8533 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/metadata.md
+-rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/path-operation-configuration.md
+-rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/path-params-numeric-validations.md
+-rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0    38884 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/query-params-str-validations.md
+-rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0    31261 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/response-model.md
+-rw-r--r--   0        0        0     7166 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/response-status-code.md
+-rw-r--r--   0        0        0    11861 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/schema-extra-example.md
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/static-files.md
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/ru/docs/tutorial/testing.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/tr/mkdocs.yml
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/tr/docs/benchmarks.md
+-rw-r--r--   0        0        0     6914 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/tr/docs/fastapi-people.md
+-rw-r--r--   0        0        0    11579 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/tr/docs/features.md
+-rw-r--r--   0        0        0    20543 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/tr/docs/index.md
+-rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/tr/docs/python-types.md
+-rw-r--r--   0        0        0    10004 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/tr/docs/tutorial/first_steps.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/mkdocs.yml
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/benchmarks.md
+-rw-r--r--   0        0        0    13647 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/contributing.md
+-rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/fastapi-people.md
+-rw-r--r--   0        0        0     9335 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/features.md
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/help-fastapi.md
+-rw-r--r--   0        0        0    18357 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/index.md
+-rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/python-types.md
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/advanced/additional-status-codes.md
+-rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/advanced/custom-response.md
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/advanced/index.md
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/advanced/path-operation-advanced-configuration.md
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/advanced/response-change-status-code.md
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/advanced/response-cookies.md
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/advanced/response-directly.md
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/advanced/response-headers.md
+-rw-r--r--   0        0        0    14283 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/advanced/settings.md
+-rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/advanced/websockets.md
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/advanced/wsgi.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/advanced/security/index.md
+-rw-r--r--   0        0        0    18647 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/bigger-applications.md
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/body-fields.md
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/body-multiple-params.md
+-rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/body-nested-models.md
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/body-updates.md
+-rw-r--r--   0        0        0     5620 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/body.md
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/cookie-params.md
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/cors.md
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/debugging.md
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/encoder.md
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/extra-data-types.md
+-rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/extra-models.md
+-rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/handling-errors.md
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/header-params.md
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/index.md
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/metadata.md
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/middleware.md
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/path-operation-configuration.md
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/path-params-numeric-validations.md
+-rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/path-params.md
+-rw-r--r--   0        0        0     9302 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/query-params-str-validations.md
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/query-params.md
+-rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/request-files.md
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/request-forms-and-files.md
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/request-forms.md
+-rw-r--r--   0        0        0     7297 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/response-model.md
+-rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/response-status-code.md
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/schema-extra-example.md
+-rw-r--r--   0        0        0    27546 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/sql-databases.md
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/static-files.md
+-rw-r--r--   0        0        0     6107 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/testing.md
+-rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/dependencies/classes-as-dependencies.md
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/dependencies/global-dependencies.md
+-rw-r--r--   0        0        0     7190 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/dependencies/index.md
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/dependencies/sub-dependencies.md
+-rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/security/first-steps.md
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/security/get-current-user.md
+-rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/security/index.md
+-rw-r--r--   0        0        0     9457 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/security/oauth2-jwt.md
+-rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs/zh/docs/tutorial/security/simple-oauth2.md
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/additional_responses/tutorial001.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/additional_responses/tutorial002.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/additional_responses/tutorial003.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/additional_responses/tutorial004.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/additional_status_codes/tutorial001.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/additional_status_codes/tutorial001_an.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/additional_status_codes/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/additional_status_codes/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/additional_status_codes/tutorial001_py310.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/advanced_middleware/tutorial001.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/advanced_middleware/tutorial002.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/advanced_middleware/tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/main.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/test_main.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/tutorial001.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/tutorial002.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/app_b/__init__.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/app_b/main.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/app_b/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/app_b_an/__init__.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/app_b_an/main.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/app_b_an/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/app_b_an_py310/__init__.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/app_b_an_py310/main.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/app_b_an_py310/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/app_b_an_py39/__init__.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/app_b_an_py39/main.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/app_b_an_py39/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/app_b_py310/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/app_b_py310/main.py
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/app_testing/app_b_py310/test_main.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/async_sql_databases/tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/async_tests/__init__.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/async_tests/main.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/async_tests/test_main.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/background_tasks/tutorial001.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/background_tasks/tutorial002.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/background_tasks/tutorial002_an.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/background_tasks/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/background_tasks/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/background_tasks/tutorial002_py310.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/behind_a_proxy/tutorial001.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/behind_a_proxy/tutorial002.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/behind_a_proxy/tutorial003.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/behind_a_proxy/tutorial004.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app/__init__.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app/dependencies.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app/internal/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app/internal/admin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app/routers/__init__.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app/routers/items.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app/routers/users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app_an/__init__.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app_an/dependencies.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app_an/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app_an/internal/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app_an/internal/admin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app_an/routers/__init__.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app_an/routers/items.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app_an/routers/users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app_an_py39/__init__.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app_an_py39/dependencies.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app_an_py39/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app_an_py39/internal/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app_an_py39/internal/admin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app_an_py39/routers/__init__.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app_an_py39/routers/items.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/bigger_applications/app_an_py39/routers/users.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body/tutorial001.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body/tutorial001_py310.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body/tutorial002.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body/tutorial002_py310.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body/tutorial003.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body/tutorial003_py310.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body/tutorial004.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body/tutorial004_py310.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_fields/tutorial001.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_fields/tutorial001_an.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_fields/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_fields/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_fields/tutorial001_py310.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial001.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial001_an.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial001_py310.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial002.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial002_py310.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial003.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial003_an.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial003_py310.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial004.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial004_an.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial004_py310.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial005.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial005_an.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial005_an_py310.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_multiple_params/tutorial005_py310.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial001.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial001_py310.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial002.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial002_py310.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial002_py39.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial003.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial003_py310.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial003_py39.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial004.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial004_py310.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial004_py39.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial005.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial005_py310.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial005_py39.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial006.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial006_py310.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial006_py39.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial007.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial007_py310.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial007_py39.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial008.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial008_py39.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial009.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_nested_models/tutorial009_py39.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_updates/tutorial001.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_updates/tutorial001_py310.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_updates/tutorial001_py39.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_updates/tutorial002.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_updates/tutorial002_py310.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/body_updates/tutorial002_py39.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/conditional_openapi/tutorial001.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/cookie_params/tutorial001.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/cookie_params/tutorial001_an.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/cookie_params/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/cookie_params/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/cookie_params/tutorial001_py310.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/cors/tutorial001.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/custom_request_and_route/tutorial001.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/custom_request_and_route/tutorial002.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/custom_request_and_route/tutorial003.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/custom_response/tutorial001.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/custom_response/tutorial001b.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/custom_response/tutorial002.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/custom_response/tutorial003.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/custom_response/tutorial004.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/custom_response/tutorial005.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/custom_response/tutorial006.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/custom_response/tutorial006b.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/custom_response/tutorial006c.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/custom_response/tutorial007.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/custom_response/tutorial008.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/custom_response/tutorial009.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/custom_response/tutorial009b.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/custom_response/tutorial009c.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/custom_response/tutorial010.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dataclasses/tutorial001.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dataclasses/tutorial002.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dataclasses/tutorial003.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/debugging/tutorial001.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial001.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial001_02_an.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial001_02_an_py310.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial001_02_an_py39.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial001_an.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial001_py310.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial002.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial002_an.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial002_py310.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial003.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial003_an.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial003_py310.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial004.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial004_an.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial004_py310.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial005.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial005_an.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial005_an_py310.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial005_py310.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial006.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial006_an.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial006_an_py39.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial007.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial008.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial008_an.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial008_an_py39.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial009.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial010.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial011.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial011_an.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial011_an_py39.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial012.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial012_an.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependencies/tutorial012_an_py39.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependency_testing/tutorial001.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependency_testing/tutorial001_an.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependency_testing/tutorial001_an_py310.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependency_testing/tutorial001_an_py39.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/dependency_testing/tutorial001_py310.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/encoder/tutorial001.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/encoder/tutorial001_py310.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/events/tutorial001.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/events/tutorial002.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/events/tutorial003.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extending_openapi/tutorial001.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extending_openapi/tutorial002.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extending_openapi/tutorial003.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extending_openapi/tutorial004.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extending_openapi/tutorial005.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extra_data_types/tutorial001.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extra_data_types/tutorial001_an.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extra_data_types/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extra_data_types/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extra_data_types/tutorial001_py310.py
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extra_models/tutorial001.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extra_models/tutorial001_py310.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extra_models/tutorial002.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extra_models/tutorial002_py310.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extra_models/tutorial003.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extra_models/tutorial003_py310.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extra_models/tutorial004.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extra_models/tutorial004_py39.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extra_models/tutorial005.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/extra_models/tutorial005_py39.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/first_steps/tutorial001.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/first_steps/tutorial002.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/first_steps/tutorial003.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/generate_clients/tutorial001.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/generate_clients/tutorial001_py39.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/generate_clients/tutorial002.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/generate_clients/tutorial002_py39.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/generate_clients/tutorial003.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/generate_clients/tutorial003_py39.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/generate_clients/tutorial004.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/graphql/tutorial001.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/handling_errors/tutorial001.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/handling_errors/tutorial002.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/handling_errors/tutorial003.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/handling_errors/tutorial004.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/handling_errors/tutorial005.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/handling_errors/tutorial006.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/header_params/tutorial001.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/header_params/tutorial001_an.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/header_params/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/header_params/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/header_params/tutorial001_py310.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/header_params/tutorial002.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/header_params/tutorial002_an.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/header_params/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/header_params/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/header_params/tutorial002_py310.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/header_params/tutorial003.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/header_params/tutorial003_an.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/header_params/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/header_params/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/header_params/tutorial003_py310.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/header_params/tutorial003_py39.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/metadata/tutorial001.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/metadata/tutorial001_1.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/metadata/tutorial002.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/metadata/tutorial003.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/metadata/tutorial004.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/middleware/tutorial001.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/nosql_databases/tutorial001.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/openapi_callbacks/tutorial001.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/openapi_webhooks/tutorial001.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_advanced_configuration/tutorial001.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_advanced_configuration/tutorial002.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_advanced_configuration/tutorial003.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_advanced_configuration/tutorial004.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_advanced_configuration/tutorial005.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_advanced_configuration/tutorial006.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_advanced_configuration/tutorial007.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_configuration/tutorial001.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_configuration/tutorial001_py310.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_configuration/tutorial001_py39.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_configuration/tutorial002.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_configuration/tutorial002_py310.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_configuration/tutorial002_py39.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_configuration/tutorial002b.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_configuration/tutorial003.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_configuration/tutorial003_py310.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_configuration/tutorial003_py39.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_configuration/tutorial004.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_configuration/tutorial004_py310.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_configuration/tutorial004_py39.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_configuration/tutorial005.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_configuration/tutorial005_py310.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_configuration/tutorial005_py39.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_operation_configuration/tutorial006.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params/tutorial001.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params/tutorial002.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params/tutorial003.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params/tutorial003b.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params/tutorial004.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params/tutorial005.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial001.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial001_an.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial001_an_py310.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial001_py310.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial002.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial002_an.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial003.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial003_an.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial004.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial004_an.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial005.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial005_an.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial006.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial006_an.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/path_params_numeric_validations/tutorial006_an_py39.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial001.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial002.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial003.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial004.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial005.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial006.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial006_py39.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial007.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial007_py39.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial008.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial008_py39.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial008b.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial008b_py310.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial009.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial009_py310.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial009b.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial009c.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial009c_py310.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial010.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial011.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial011_py310.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial011_py39.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial012.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial013.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/python_types/tutorial013_py39.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params/tutorial001.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params/tutorial002.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params/tutorial002_py310.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params/tutorial003.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params/tutorial003_py310.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params/tutorial004.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params/tutorial004_py310.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params/tutorial005.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params/tutorial006.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params/tutorial006_py310.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params/tutorial006b.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial001.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial001_py310.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial002.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial002_an.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial002_py310.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial003.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial003_an.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial003_py310.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial004.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial004_an.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial004_py310.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial005.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial005_an.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial005_an_py39.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial006.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial006_an.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial006_an_py39.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial006b.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial006b_an.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial006b_an_py39.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial006c.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial006c_an.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial006c_an_py310.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial006c_an_py39.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial006c_py310.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial006d.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial006d_an.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial006d_an_py39.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial007.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial007_an.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial007_an_py310.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial007_an_py39.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial007_py310.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial008.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial008_an.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial008_an_py310.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial008_an_py39.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial008_py310.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial009.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial009_an.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial009_an_py310.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial009_an_py39.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial009_py310.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial010.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial010_an.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial010_an_py310.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial010_an_py39.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial010_py310.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial011.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial011_an.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial011_an_py310.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial011_an_py39.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial011_py310.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial011_py39.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial012.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial012_an.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial012_an_py39.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial012_py39.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial013.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial013_an.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial013_an_py39.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial014.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial014_an.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial014_an_py310.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial014_an_py39.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/query_params_str_validations/tutorial014_py310.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_files/tutorial001.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_files/tutorial001_02.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_files/tutorial001_02_an.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_files/tutorial001_02_an_py310.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_files/tutorial001_02_an_py39.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_files/tutorial001_02_py310.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_files/tutorial001_03.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_files/tutorial001_03_an.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_files/tutorial001_03_an_py39.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_files/tutorial001_an.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_files/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_files/tutorial002.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_files/tutorial002_an.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_files/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_files/tutorial002_py39.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_files/tutorial003.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_files/tutorial003_an.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_files/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_files/tutorial003_py39.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_forms/tutorial001.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_forms/tutorial001_an.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_forms/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_forms_and_files/tutorial001.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_forms_and_files/tutorial001_an.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/request_forms_and_files/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_change_status_code/tutorial001.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_cookies/tutorial001.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_cookies/tutorial002.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_directly/tutorial001.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_directly/tutorial002.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_headers/tutorial001.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_headers/tutorial002.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial001.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial001_01.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial001_01_py310.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial001_01_py39.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial001_py310.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial001_py39.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial002.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial002_py310.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial003.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial003_01.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial003_01_py310.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial003_02.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial003_03.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial003_04.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial003_04_py310.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial003_05.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial003_05_py310.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial003_py310.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial004.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial004_py310.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial004_py39.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial005.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial005_py310.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial006.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_model/tutorial006_py310.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_status_code/tutorial001.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/response_status_code/tutorial002.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/schema_extra_example/tutorial001.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/schema_extra_example/tutorial001_py310.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/schema_extra_example/tutorial002.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/schema_extra_example/tutorial002_py310.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/schema_extra_example/tutorial003.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/schema_extra_example/tutorial003_an.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/schema_extra_example/tutorial003_an_py310.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/schema_extra_example/tutorial003_an_py39.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/schema_extra_example/tutorial003_py310.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/schema_extra_example/tutorial004.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/schema_extra_example/tutorial004_an.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/schema_extra_example/tutorial004_an_py310.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/schema_extra_example/tutorial004_an_py39.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/schema_extra_example/tutorial004_py310.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial001.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial001_an.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial001_an_py39.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial002.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial002_an.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial002_an_py310.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial002_an_py39.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial002_py310.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial003.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial003_an.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial003_an_py310.py
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial003_an_py39.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial003_py310.py
+-rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial004.py
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial004_an.py
+-rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial004_an_py310.py
+-rw-r--r--   0        0        0     4198 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial004_an_py39.py
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial004_py310.py
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial005.py
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial005_an.py
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial005_an_py310.py
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial005_an_py39.py
+-rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial005_py310.py
+-rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial005_py39.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial006.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial006_an.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial006_an_py39.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial007.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial007_an.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/security/tutorial007_an_py39.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app01/__init__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app01/config.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app01/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app02/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app02/config.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app02/main.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app02/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app02_an/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app02_an/config.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app02_an/main.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app02_an/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app02_an_py39/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app02_an_py39/config.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app02_an_py39/main.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app02_an_py39/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app03/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app03/config.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app03/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app03_an/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app03_an/config.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app03_an/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app03_an_py39/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app03_an_py39/config.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/settings/app03_an_py39/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app/__init__.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app/alt_main.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app/crud.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app/database.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app/main.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app/models.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app/tests/__init__.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app/tests/test_sql_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app_py310/__init__.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app_py310/alt_main.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app_py310/crud.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app_py310/database.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app_py310/main.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app_py310/models.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app_py310/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app_py310/tests/__init__.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app_py39/__init__.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app_py39/alt_main.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app_py39/crud.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app_py39/database.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app_py39/main.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app_py39/models.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app_py39/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app_py39/tests/__init__.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases_peewee/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases_peewee/sql_app/__init__.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases_peewee/sql_app/crud.py
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases_peewee/sql_app/database.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases_peewee/sql_app/main.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases_peewee/sql_app/models.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sql_databases_peewee/sql_app/schemas.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/static_files/tutorial001.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/sub_applications/tutorial001.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/templates/tutorial001.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/templates/static/styles.css
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/templates/templates/item.html
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/using_request_directly/tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/websockets/__init__.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/websockets/tutorial001.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/websockets/tutorial002.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/websockets/tutorial002_an.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/websockets/tutorial002_an_py310.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/websockets/tutorial002_an_py39.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/websockets/tutorial002_py310.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/websockets/tutorial003.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/websockets/tutorial003_py39.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 fastapi-0.99.1/docs_src/wsgi/tutorial001.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/__init__.py
+-rw-r--r--   0        0        0    40588 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/applications.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/background.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/concurrency.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/datastructures.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/encoders.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/exception_handlers.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/exceptions.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/logger.py
+-rw-r--r--   0        0        0     8981 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/param_functions.py
+-rw-r--r--   0        0        0    13207 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/py.typed
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/requests.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/responses.py
+-rw-r--r--   0        0        0    56490 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/routing.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/staticfiles.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/templating.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/testclient.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/types.py
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/utils.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/websockets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/dependencies/__init__.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/dependencies/models.py
+-rw-r--r--   0        0        0    30908 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/dependencies/utils.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/middleware/__init__.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/middleware/cors.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/middleware/gzip.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/middleware/httpsredirect.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/middleware/trustedhost.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/openapi/__init__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/openapi/constants.py
+-rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/openapi/docs.py
+-rw-r--r--   0        0        0    14941 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/openapi/models.py
+-rw-r--r--   0        0        0    19576 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/openapi/utils.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/security/__init__.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/security/api_key.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/security/base.py
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/security/http.py
+-rw-r--r--   0        0        0     8360 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/security/oauth2.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/security/open_id_connect_url.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 fastapi-0.99.1/fastapi/security/utils.py
+-rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 fastapi-0.99.1/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 fastapi-0.99.1/scripts/clean.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 fastapi-0.99.1/scripts/docs-live.sh
+-rw-r--r--   0        0        0     9995 2020-02-02 00:00:00.000000 fastapi-0.99.1/scripts/docs.py
+-rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 fastapi-0.99.1/scripts/format.sh
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 fastapi-0.99.1/scripts/gitter_releases_bot.py
+-rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 fastapi-0.99.1/scripts/lint.sh
+-rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 fastapi-0.99.1/scripts/mkdocs_hooks.py
+-rwxr-xr-x   0        0        0      337 2020-02-02 00:00:00.000000 fastapi-0.99.1/scripts/netlify-docs.sh
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 fastapi-0.99.1/scripts/notify.sh
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 fastapi-0.99.1/scripts/publish.sh
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 fastapi-0.99.1/scripts/test-cov-html.sh
+-rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 fastapi-0.99.1/scripts/test.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/__init__.py
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/main.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_additional_properties.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_additional_properties_bool.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_additional_response_extra.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_additional_responses_bad.py
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_additional_responses_custom_model_in_callback.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_additional_responses_custom_validationerror.py
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_additional_responses_default_validationerror.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_additional_responses_response_class.py
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_additional_responses_router.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_ambiguous_params.py
+-rw-r--r--   0        0        0     9779 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_annotated.py
+-rw-r--r--   0        0        0    49052 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_application.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_callable_endpoint.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_custom_middleware_exception.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_custom_route_class.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_custom_schema_fields.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_custom_swagger_ui_redirect.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_datastructures.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_datetime_custom_encoder.py
+-rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_default_response_class.py
+-rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_default_response_class_router.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_dependency_cache.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_dependency_class.py
+-rw-r--r--   0        0        0    11269 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_dependency_contextmanager.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_dependency_contextvars.py
+-rw-r--r--   0        0        0     8164 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_dependency_duplicates.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_dependency_normal_exceptions.py
+-rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_dependency_overrides.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_dependency_security_overrides.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_deprecated_openapi_prefix.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_duplicate_models_openapi.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_empty_router.py
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_enforce_once_required_parameter.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_exception_handlers.py
+-rw-r--r--   0        0        0    13670 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_extra_routes.py
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_filter_pydantic_sub_model.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_forms_from_non_typing_sequences.py
+-rw-r--r--   0        0        0    68172 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_generate_unique_id_function.py
+-rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_get_request_body.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_http_connection_injection.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_include_route.py
+-rw-r--r--   0        0        0   367192 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_include_router_defaults_overrides.py
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_infer_param_optionality.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_inherited_custom_class.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_invalid_path_param.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_invalid_sequence_param.py
+-rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_jsonable_encoder.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_local_docs.py
+-rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_multi_body_errors.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_multi_query_errors.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_multipart_installation.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_no_swagger_ui_redirect.py
+-rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_openapi_query_parameter_extension.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_openapi_route_extensions.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_openapi_servers.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_operations_signatures.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_orjson_response_class.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_param_class.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_param_in_path_and_dependency.py
+-rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_param_include_in_schema.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_params_repr.py
+-rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_path.py
+-rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_put_no_body.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_query.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_read_with_orm_mode.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_repeated_cookie_headers.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_repeated_dependency_schema.py
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_repeated_parameter_alias.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_reponse_set_reponse_code_empty.py
+-rw-r--r--   0        0        0     6546 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_request_body_parameters_media_type.py
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_required_noneable.py
+-rw-r--r--   0        0        0    10951 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_response_by_alias.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_response_change_status_code.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_response_class_no_mediatype.py
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_response_code_no_body.py
+-rw-r--r--   0        0        0    48457 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_response_model_as_return_annotation.py
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_response_model_include_exclude.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_response_model_invalid.py
+-rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_response_model_sub_types.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_route_scope.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_router_events.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_router_prefix_with_template.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_router_redirect_slashes.py
+-rw-r--r--   0        0        0    32406 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_schema_extra_examples.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_api_key_cookie.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_api_key_cookie_description.py
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_api_key_cookie_optional.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_api_key_header.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_api_key_header_description.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_api_key_header_optional.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_api_key_query.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_api_key_query_description.py
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_api_key_query_optional.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_http_base.py
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_http_base_description.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_http_base_optional.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_http_basic_optional.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_http_basic_realm.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_http_basic_realm_description.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_http_bearer.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_http_bearer_description.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_http_bearer_optional.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_http_digest.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_http_digest_description.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_http_digest_optional.py
+-rw-r--r--   0        0        0     8340 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_oauth2.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_oauth2_authorization_code_bearer.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_oauth2_authorization_code_bearer_description.py
+-rw-r--r--   0        0        0     8387 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_oauth2_optional.py
+-rw-r--r--   0        0        0     8490 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_oauth2_optional_description.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_oauth2_password_bearer_optional.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_oauth2_password_bearer_optional_description.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_openid_connect.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_openid_connect_description.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_security_openid_connect_optional.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_serialize_response.py
+-rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_serialize_response_dataclass.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_serialize_response_model.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_skip_defaults.py
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_starlette_exception.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_starlette_urlconvertors.py
+-rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_sub_callbacks.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_swagger_ui_init_oauth.py
+-rw-r--r--   0        0        0     9847 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tuples.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_typing_python39.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_union_body.py
+-rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_union_inherited_body.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_validate_response.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_validate_response_dataclass.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_validate_response_recursive.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_webhooks_security.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_ws_dependencies.py
+-rw-r--r--   0        0        0     7651 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_ws_router.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_modules_same_name_body/__init__.py
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_modules_same_name_body/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_modules_same_name_body/app/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_modules_same_name_body/app/a.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_modules_same_name_body/app/b.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_modules_same_name_body/app/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_additional_responses/__init__.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_additional_responses/test_tutorial001.py
+-rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_additional_responses/test_tutorial002.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_additional_responses/test_tutorial003.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_additional_responses/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_additional_status_codes/__init__.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_advanced_middleware/__init__.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_advanced_middleware/test_tutorial001.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_async_sql_databases/__init__.py
+-rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_async_tests/__init__.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_async_tests/test_main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_background_tasks/__init__.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_background_tasks/test_tutorial001.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_background_tasks/test_tutorial002.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_behind_a_proxy/__init__.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_bigger_applications/__init__.py
+-rw-r--r--   0        0        0    18714 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_bigger_applications/test_main.py
+-rw-r--r--   0        0        0    18717 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_bigger_applications/test_main_an.py
+-rw-r--r--   0        0        0    19078 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body/__init__.py
+-rw-r--r--   0        0        0     8723 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body/test_tutorial001.py
+-rw-r--r--   0        0        0     9101 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_fields/__init__.py
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_fields/test_tutorial001.py
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_fields/test_tutorial001_an.py
+-rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/__init__.py
+-rw-r--r--   0        0        0     5239 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py
+-rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py
+-rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py
+-rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py
+-rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py
+-rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_nested_models/__init__.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_nested_models/test_tutorial009.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_updates/__init__.py
+-rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_updates/test_tutorial001.py
+-rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     6248 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_conditional_openapi/__init__.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_cookie_params/__init__.py
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_cookie_params/test_tutorial001.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_cors/__init__.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_cors/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_custom_request_and_route/__init__.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_custom_response/__init__.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_custom_response/test_tutorial001.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_custom_response/test_tutorial001b.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_custom_response/test_tutorial004.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_custom_response/test_tutorial005.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_custom_response/test_tutorial006.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_custom_response/test_tutorial006b.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_custom_response/test_tutorial006c.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_custom_response/test_tutorial007.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_custom_response/test_tutorial008.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_custom_response/test_tutorial009.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_custom_response/test_tutorial009b.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_custom_response/test_tutorial009c.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dataclasses/__init__.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dataclasses/test_tutorial001.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dataclasses/test_tutorial002.py
+-rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dataclasses/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dependencies/__init__.py
+-rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial001.py
+-rw-r--r--   0        0        0     6356 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial001_an.py
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial004.py
+-rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial004_an.py
+-rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py
+-rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial006.py
+-rw-r--r--   0        0        0     4480 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial006_an.py
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py
+-rw-r--r--   0        0        0     7386 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial012.py
+-rw-r--r--   0        0        0     7389 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial012_an.py
+-rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_events/__init__.py
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_events/test_tutorial001.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_events/test_tutorial002.py
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_events/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_extending_openapi/__init__.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_extending_openapi/test_tutorial001.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_extending_openapi/test_tutorial002.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_extending_openapi/test_tutorial003.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_extending_openapi/test_tutorial004.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_extending_openapi/test_tutorial005.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_extra_data_types/__init__.py
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_extra_data_types/test_tutorial001.py
+-rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py
+-rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     5365 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_extra_models/__init__.py
+-rw-r--r--   0        0        0     4808 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_extra_models/test_tutorial003.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_extra_models/test_tutorial004.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_extra_models/test_tutorial005.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_first_steps/__init__.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_first_steps/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_generate_clients/__init__.py
+-rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_generate_clients/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_handling_errors/__init__.py
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_handling_errors/test_tutorial001.py
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_handling_errors/test_tutorial002.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_handling_errors/test_tutorial003.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_handling_errors/test_tutorial004.py
+-rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_handling_errors/test_tutorial005.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_handling_errors/test_tutorial006.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_header_params/__init__.py
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial001.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial001_an.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial001_py310.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial002.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial002_an.py
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py
+-rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial002_py310.py
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial003.py
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial003_an.py
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial003_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_metadata/__init__.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_metadata/test_tutorial001.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_metadata/test_tutorial001_1.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_metadata/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_openapi_callbacks/__init__.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_openapi_webhooks/__init__.py
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_openapi_webhooks/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_path_operation_advanced_configurations/__init__.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_path_operation_configurations/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py
+-rw-r--r--   0        0        0     4682 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_path_params/__init__.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_path_params/test_tutorial004.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_path_params/test_tutorial005.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params/__init__.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params/test_tutorial005.py
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params/test_tutorial006.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params/test_tutorial006_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/__init__.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py
+-rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py
+-rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/__init__.py
+-rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001.py
+-rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_02.py
+-rw-r--r--   0        0        0     5987 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py
+-rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py
+-rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py
+-rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py
+-rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_03.py
+-rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py
+-rw-r--r--   0        0        0     6300 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py
+-rw-r--r--   0        0        0     6735 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_an.py
+-rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     7703 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial002.py
+-rw-r--r--   0        0        0     7706 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial002_an.py
+-rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial002_py39.py
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial003.py
+-rw-r--r--   0        0        0     7314 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial003_an.py
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     7827 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial003_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_forms/__init__.py
+-rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_forms/test_tutorial001.py
+-rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_forms/test_tutorial001_an.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_forms_and_files/__init__.py
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py
+-rw-r--r--   0        0        0     6418 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py
+-rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_change_status_code/__init__.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_cookies/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_cookies/test_tutorial001.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_cookies/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_headers/__init__.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_headers/test_tutorial001.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_headers/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_model/__init__.py
+-rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial003.py
+-rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial003_01.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial003_02.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial003_03.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial003_04.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial003_04_py310.py
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial003_05.py
+-rw-r--r--   0        0        0     3699 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py
+-rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial003_py310.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial004.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial004_py310.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial004_py39.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial005.py
+-rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial005_py310.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial006.py
+-rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial006_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_schema_extra_example/__init__.py
+-rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py
+-rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py
+-rw-r--r--   0        0        0     5133 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_security/__init__.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial001.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial001_an.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     6832 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial003.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial003_an.py
+-rw-r--r--   0        0        0     7244 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial003_an_py310.py
+-rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial003_an_py39.py
+-rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial003_py310.py
+-rw-r--r--   0        0        0    13084 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial005.py
+-rw-r--r--   0        0        0    13087 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial005_an.py
+-rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial005_an_py310.py
+-rw-r--r--   0        0        0    13968 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial005_an_py39.py
+-rw-r--r--   0        0        0    13980 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial005_py310.py
+-rw-r--r--   0        0        0    13956 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial005_py39.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial006.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial006_an.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial006_an_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_settings/__init__.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_settings/test_app02.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_sql_databases/__init__.py
+-rw-r--r--   0        0        0    15205 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_sql_databases/test_sql_databases.py
+-rw-r--r--   0        0        0    15384 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py
+-rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py
+-rw-r--r--   0        0        0    15666 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py
+-rw-r--r--   0        0        0    15681 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py
+-rw-r--r--   0        0        0    15672 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_sql_databases/test_testing_databases.py
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_sql_databases_peewee/__init__.py
+-rw-r--r--   0        0        0    17654 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_sql_databases_peewee/test_sql_databases_peewee.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_sub_applications/__init__.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_sub_applications/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_templates/__init__.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_templates/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_testing/__init__.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_testing/test_main.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_testing/test_main_b.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_testing/test_main_b_an.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_testing/test_main_b_an_py310.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_testing/test_main_b_an_py39.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_testing/test_main_b_py310.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_testing/test_tutorial001.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_testing/test_tutorial002.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_testing/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_testing_dependencies/__init__.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py
+-rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_websockets/__init__.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_websockets/test_tutorial001.py
+-rw-r--r--   0        0        0     3683 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_websockets/test_tutorial002.py
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_websockets/test_tutorial002_an.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_websockets/test_tutorial002_py310.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_websockets/test_tutorial003.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_websockets/test_tutorial003_py39.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_wsgi/__init__.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 fastapi-0.99.1/tests/test_tutorial/test_wsgi/test_tutorial001.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 fastapi-0.99.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 fastapi-0.99.1/LICENSE
+-rw-r--r--   0        0        0    20581 2020-02-02 00:00:00.000000 fastapi-0.99.1/README.md
+-rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 fastapi-0.99.1/pyproject.toml
+-rw-r--r--   0        0        0    23001 2020-02-02 00:00:00.000000 fastapi-0.99.1/PKG-INFO
```

### Comparing `fastapi-0.99.0/.pre-commit-config.yaml` & `fastapi-0.99.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/SECURITY.md` & `fastapi-0.99.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/requirements-tests.txt` & `fastapi-0.99.1/requirements-tests.txt`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/.github/DISCUSSION_TEMPLATE/questions.yml` & `fastapi-0.99.1/.github/DISCUSSION_TEMPLATE/questions.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/.github/ISSUE_TEMPLATE/config.yml` & `fastapi-0.99.1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/.github/ISSUE_TEMPLATE/privileged.yml` & `fastapi-0.99.1/.github/ISSUE_TEMPLATE/privileged.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/.github/actions/comment-docs-preview-in-pr/app/main.py` & `fastapi-0.99.1/.github/actions/comment-docs-preview-in-pr/app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/.github/actions/notify-translations/app/main.py` & `fastapi-0.99.1/.github/actions/notify-translations/app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/.github/actions/people/app/main.py` & `fastapi-0.99.1/.github/actions/people/app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/.github/workflows/build-docs.yml` & `fastapi-0.99.1/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/.github/workflows/deploy-docs.yml` & `fastapi-0.99.1/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/.github/workflows/issue-manager.yml` & `fastapi-0.99.1/.github/workflows/issue-manager.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/.github/workflows/latest-changes.yml` & `fastapi-0.99.1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/.github/workflows/notify-translations.yml` & `fastapi-0.99.1/.github/workflows/notify-translations.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/.github/workflows/people.yml` & `fastapi-0.99.1/.github/workflows/people.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/.github/workflows/publish.yml` & `fastapi-0.99.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/.github/workflows/smokeshow.yml` & `fastapi-0.99.1/.github/workflows/smokeshow.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/.github/workflows/test.yml` & `fastapi-0.99.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/de/docs/features.md` & `fastapi-0.99.1/docs/de/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/alternatives.md` & `fastapi-0.99.1/docs/em/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/async.md` & `fastapi-0.99.1/docs/em/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/benchmarks.md` & `fastapi-0.99.1/docs/em/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/contributing.md` & `fastapi-0.99.1/docs/em/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/external-links.md` & `fastapi-0.99.1/docs/em/docs/external-links.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/fastapi-people.md` & `fastapi-0.99.1/docs/em/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/features.md` & `fastapi-0.99.1/docs/em/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/help-fastapi.md` & `fastapi-0.99.1/docs/em/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/history-design-future.md` & `fastapi-0.99.1/docs/em/docs/history-design-future.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/index.md` & `fastapi-0.99.1/docs/em/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/project-generation.md` & `fastapi-0.99.1/docs/em/docs/project-generation.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/python-types.md` & `fastapi-0.99.1/docs/em/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/additional-responses.md` & `fastapi-0.99.1/docs/em/docs/advanced/additional-responses.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/additional-status-codes.md` & `fastapi-0.99.1/docs/em/docs/advanced/additional-status-codes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/advanced-dependencies.md` & `fastapi-0.99.1/docs/em/docs/advanced/advanced-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/async-sql-databases.md` & `fastapi-0.99.1/docs/em/docs/advanced/async-sql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/async-tests.md` & `fastapi-0.99.1/docs/em/docs/advanced/async-tests.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/behind-a-proxy.md` & `fastapi-0.99.1/docs/em/docs/advanced/behind-a-proxy.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/conditional-openapi.md` & `fastapi-0.99.1/docs/em/docs/advanced/conditional-openapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/custom-request-and-route.md` & `fastapi-0.99.1/docs/em/docs/advanced/custom-request-and-route.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/custom-response.md` & `fastapi-0.99.1/docs/em/docs/advanced/custom-response.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/dataclasses.md` & `fastapi-0.99.1/docs/em/docs/advanced/dataclasses.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/events.md` & `fastapi-0.99.1/docs/em/docs/advanced/events.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/extending-openapi.md` & `fastapi-0.99.1/docs/em/docs/advanced/extending-openapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/generate-clients.md` & `fastapi-0.99.1/docs/em/docs/advanced/generate-clients.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/graphql.md` & `fastapi-0.99.1/docs/em/docs/advanced/graphql.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/index.md` & `fastapi-0.99.1/docs/em/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/middleware.md` & `fastapi-0.99.1/docs/em/docs/advanced/middleware.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/nosql-databases.md` & `fastapi-0.99.1/docs/em/docs/advanced/nosql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/openapi-callbacks.md` & `fastapi-0.99.1/docs/em/docs/advanced/openapi-callbacks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/path-operation-advanced-configuration.md` & `fastapi-0.99.1/docs/em/docs/advanced/path-operation-advanced-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/response-change-status-code.md` & `fastapi-0.99.1/docs/em/docs/advanced/response-change-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/response-cookies.md` & `fastapi-0.99.1/docs/em/docs/advanced/response-cookies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/response-directly.md` & `fastapi-0.99.1/docs/em/docs/advanced/response-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/response-headers.md` & `fastapi-0.99.1/docs/em/docs/advanced/response-headers.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/settings.md` & `fastapi-0.99.1/docs/em/docs/advanced/settings.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/sql-databases-peewee.md` & `fastapi-0.99.1/docs/em/docs/advanced/sql-databases-peewee.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/sub-applications.md` & `fastapi-0.99.1/docs/em/docs/advanced/sub-applications.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/templates.md` & `fastapi-0.99.1/docs/em/docs/advanced/templates.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/testing-database.md` & `fastapi-0.99.1/docs/em/docs/advanced/testing-database.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/testing-dependencies.md` & `fastapi-0.99.1/docs/em/docs/advanced/testing-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/using-request-directly.md` & `fastapi-0.99.1/docs/em/docs/advanced/using-request-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/websockets.md` & `fastapi-0.99.1/docs/em/docs/advanced/websockets.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/wsgi.md` & `fastapi-0.99.1/docs/em/docs/advanced/wsgi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/security/http-basic-auth.md` & `fastapi-0.99.1/docs/em/docs/advanced/security/http-basic-auth.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/advanced/security/oauth2-scopes.md` & `fastapi-0.99.1/docs/em/docs/advanced/security/oauth2-scopes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/deployment/concepts.md` & `fastapi-0.99.1/docs/em/docs/deployment/concepts.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/deployment/deta.md` & `fastapi-0.99.1/docs/em/docs/deployment/deta.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/deployment/docker.md` & `fastapi-0.99.1/docs/em/docs/deployment/docker.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/deployment/https.md` & `fastapi-0.99.1/docs/em/docs/deployment/https.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/deployment/index.md` & `fastapi-0.99.1/docs/em/docs/deployment/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/deployment/manually.md` & `fastapi-0.99.1/docs/em/docs/deployment/manually.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/deployment/server-workers.md` & `fastapi-0.99.1/docs/em/docs/deployment/server-workers.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/deployment/versions.md` & `fastapi-0.99.1/docs/em/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/background-tasks.md` & `fastapi-0.99.1/docs/em/docs/tutorial/background-tasks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/bigger-applications.md` & `fastapi-0.99.1/docs/em/docs/tutorial/bigger-applications.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/body-fields.md` & `fastapi-0.99.1/docs/em/docs/tutorial/body-fields.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/body-multiple-params.md` & `fastapi-0.99.1/docs/em/docs/tutorial/body-multiple-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/body-nested-models.md` & `fastapi-0.99.1/docs/em/docs/tutorial/body-nested-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/body-updates.md` & `fastapi-0.99.1/docs/em/docs/tutorial/body-updates.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/body.md` & `fastapi-0.99.1/docs/em/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/cookie-params.md` & `fastapi-0.99.1/docs/em/docs/tutorial/cookie-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/cors.md` & `fastapi-0.99.1/docs/em/docs/tutorial/cors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/debugging.md` & `fastapi-0.99.1/docs/em/docs/tutorial/debugging.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/encoder.md` & `fastapi-0.99.1/docs/em/docs/tutorial/encoder.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/extra-data-types.md` & `fastapi-0.99.1/docs/em/docs/tutorial/extra-data-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/extra-models.md` & `fastapi-0.99.1/docs/em/docs/tutorial/extra-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/first-steps.md` & `fastapi-0.99.1/docs/em/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/handling-errors.md` & `fastapi-0.99.1/docs/em/docs/tutorial/handling-errors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/header-params.md` & `fastapi-0.99.1/docs/em/docs/tutorial/header-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/index.md` & `fastapi-0.99.1/docs/em/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/metadata.md` & `fastapi-0.99.1/docs/em/docs/tutorial/metadata.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/middleware.md` & `fastapi-0.99.1/docs/em/docs/tutorial/middleware.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/path-operation-configuration.md` & `fastapi-0.99.1/docs/em/docs/tutorial/path-operation-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/path-params-numeric-validations.md` & `fastapi-0.99.1/docs/em/docs/tutorial/path-params-numeric-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/path-params.md` & `fastapi-0.99.1/docs/em/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/query-params-str-validations.md` & `fastapi-0.99.1/docs/em/docs/tutorial/query-params-str-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/query-params.md` & `fastapi-0.99.1/docs/em/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/request-files.md` & `fastapi-0.99.1/docs/em/docs/tutorial/request-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/request-forms-and-files.md` & `fastapi-0.99.1/docs/em/docs/tutorial/request-forms-and-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/request-forms.md` & `fastapi-0.99.1/docs/em/docs/tutorial/request-forms.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/response-model.md` & `fastapi-0.99.1/docs/em/docs/tutorial/response-model.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/response-status-code.md` & `fastapi-0.99.1/docs/em/docs/tutorial/response-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/schema-extra-example.md` & `fastapi-0.99.1/docs/em/docs/tutorial/schema-extra-example.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/sql-databases.md` & `fastapi-0.99.1/docs/em/docs/tutorial/sql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/static-files.md` & `fastapi-0.99.1/docs/em/docs/tutorial/static-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/testing.md` & `fastapi-0.99.1/docs/em/docs/tutorial/testing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/dependencies/classes-as-dependencies.md` & `fastapi-0.99.1/docs/em/docs/tutorial/dependencies/classes-as-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md` & `fastapi-0.99.1/docs/em/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/dependencies/dependencies-with-yield.md` & `fastapi-0.99.1/docs/em/docs/tutorial/dependencies/dependencies-with-yield.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/dependencies/global-dependencies.md` & `fastapi-0.99.1/docs/em/docs/tutorial/dependencies/global-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/dependencies/index.md` & `fastapi-0.99.1/docs/em/docs/tutorial/dependencies/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/dependencies/sub-dependencies.md` & `fastapi-0.99.1/docs/em/docs/tutorial/dependencies/sub-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/security/first-steps.md` & `fastapi-0.99.1/docs/em/docs/tutorial/security/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/security/get-current-user.md` & `fastapi-0.99.1/docs/em/docs/tutorial/security/get-current-user.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/security/index.md` & `fastapi-0.99.1/docs/em/docs/tutorial/security/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/security/oauth2-jwt.md` & `fastapi-0.99.1/docs/em/docs/tutorial/security/oauth2-jwt.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/em/docs/tutorial/security/simple-oauth2.md` & `fastapi-0.99.1/docs/em/docs/tutorial/security/simple-oauth2.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/mkdocs.yml` & `fastapi-0.99.1/docs/en/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/data/external_links.yml` & `fastapi-0.99.1/docs/en/data/external_links.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/data/github_sponsors.yml` & `fastapi-0.99.1/docs/en/data/github_sponsors.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/data/people.yml` & `fastapi-0.99.1/docs/en/data/people.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/data/sponsors.yml` & `fastapi-0.99.1/docs/en/data/sponsors.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/alternatives.md` & `fastapi-0.99.1/docs/en/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/async.md` & `fastapi-0.99.1/docs/en/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/benchmarks.md` & `fastapi-0.99.1/docs/en/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/contributing.md` & `fastapi-0.99.1/docs/en/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/external-links.md` & `fastapi-0.99.1/docs/en/docs/external-links.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/fastapi-people.md` & `fastapi-0.99.1/docs/en/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/features.md` & `fastapi-0.99.1/docs/en/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/help-fastapi.md` & `fastapi-0.99.1/docs/en/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/history-design-future.md` & `fastapi-0.99.1/docs/en/docs/history-design-future.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/index.md` & `fastapi-0.99.1/docs/en/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/project-generation.md` & `fastapi-0.99.1/docs/en/docs/project-generation.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/python-types.md` & `fastapi-0.99.1/docs/en/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/release-notes.md` & `fastapi-0.99.1/docs/en/docs/release-notes.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 # Release Notes
 
 ## Latest Changes
 
 
+## 0.99.1
+
+### Fixes
+
+* 🐛 Fix JSON Schema accepting bools as valid JSON Schemas, e.g. `additionalProperties: false`. PR [#9781](https://github.com/tiangolo/fastapi/pull/9781) by [@tiangolo](https://github.com/tiangolo).
+
+### Docs
+
+* 📝 Update source examples to use new JSON Schema examples field. PR [#9776](https://github.com/tiangolo/fastapi/pull/9776) by [@tiangolo](https://github.com/tiangolo).
+
 ## 0.99.0
 
 ### Features
 
 * ✨ Add support for OpenAPI 3.1.0. PR [#9770](https://github.com/tiangolo/fastapi/pull/9770) by [@tiangolo](https://github.com/tiangolo).
     * New support for documenting **webhooks**, read the new docs here: <a href="https://fastapi.tiangolo.com/advanced/openapi-webhooks/" class="external-link" target="_blank">Advanced User Guide: OpenAPI Webhooks</a>.
     * Upgrade OpenAPI 3.1.0, this uses JSON Schema 2020-12.
```

#### html2text {}

```diff
@@ -1,16 +1,21 @@
-# Release Notes ## Latest Changes ## 0.99.0 ### Features * â¨ Add support for
-OpenAPI 3.1.0. PR [#9770](https://github.com/tiangolo/fastapi/pull/9770) by
-[@tiangolo](https://github.com/tiangolo). * New support for documenting
-**webhooks**, read the new docs here: Advanced_User_Guide:_OpenAPI_Webhooks. *
-Upgrade OpenAPI 3.1.0, this uses JSON Schema 2020-12. * Upgrade Swagger UI to
-version 5.x.x, that supports OpenAPI 3.1.0. * Updated `examples` field in
-`Query()`, `Cookie()`, `Body()`, etc. based on the latest JSON Schema and
-OpenAPI. Now it takes a list of examples and they are included directly in the
-JSON Schema, not outside. Read more about it (including the historical
+# Release Notes ## Latest Changes ## 0.99.1 ### Fixes * ð Fix JSON Schema
+accepting bools as valid JSON Schemas, e.g. `additionalProperties: false`. PR
+[#9781](https://github.com/tiangolo/fastapi/pull/9781) by [@tiangolo](https://
+github.com/tiangolo). ### Docs * ð Update source examples to use new JSON
+Schema examples field. PR [#9776](https://github.com/tiangolo/fastapi/pull/
+9776) by [@tiangolo](https://github.com/tiangolo). ## 0.99.0 ### Features * â¨
+Add support for OpenAPI 3.1.0. PR [#9770](https://github.com/tiangolo/fastapi/
+pull/9770) by [@tiangolo](https://github.com/tiangolo). * New support for
+documenting **webhooks**, read the new docs here: Advanced_User_Guide:_OpenAPI
+Webhooks. * Upgrade OpenAPI 3.1.0, this uses JSON Schema 2020-12. * Upgrade
+Swagger UI to version 5.x.x, that supports OpenAPI 3.1.0. * Updated `examples`
+field in `Query()`, `Cookie()`, `Body()`, etc. based on the latest JSON Schema
+and OpenAPI. Now it takes a list of examples and they are included directly in
+the JSON Schema, not outside. Read more about it (including the historical
 technical details) in the updated docs: Tutorial:_Declare_Request_Example_Data.
 * â¨ Add support for `deque` objects and children in `jsonable_encoder`. PR
 [#9433](https://github.com/tiangolo/fastapi/pull/9433) by [@cranium](https://
 github.com/cranium). ### Docs * ð Fix form for the FastAPI and friends
 newsletter. PR [#9749](https://github.com/tiangolo/fastapi/pull/9749) by
 [@tiangolo](https://github.com/tiangolo). ### Translations * ð Add Persian
 translation for `docs/fa/docs/advanced/sub-applications.md`. PR [#9692](https:/
```

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/additional-responses.md` & `fastapi-0.99.1/docs/en/docs/advanced/additional-responses.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/additional-status-codes.md` & `fastapi-0.99.1/docs/en/docs/advanced/additional-status-codes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/advanced-dependencies.md` & `fastapi-0.99.1/docs/en/docs/advanced/advanced-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/async-sql-databases.md` & `fastapi-0.99.1/docs/en/docs/advanced/async-sql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/async-tests.md` & `fastapi-0.99.1/docs/en/docs/advanced/async-tests.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/behind-a-proxy.md` & `fastapi-0.99.1/docs/en/docs/advanced/behind-a-proxy.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/conditional-openapi.md` & `fastapi-0.99.1/docs/en/docs/advanced/conditional-openapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/custom-request-and-route.md` & `fastapi-0.99.1/docs/en/docs/advanced/custom-request-and-route.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/custom-response.md` & `fastapi-0.99.1/docs/en/docs/advanced/custom-response.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/dataclasses.md` & `fastapi-0.99.1/docs/en/docs/advanced/dataclasses.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/events.md` & `fastapi-0.99.1/docs/en/docs/advanced/events.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/extending-openapi.md` & `fastapi-0.99.1/docs/en/docs/advanced/extending-openapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/generate-clients.md` & `fastapi-0.99.1/docs/en/docs/advanced/generate-clients.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/graphql.md` & `fastapi-0.99.1/docs/en/docs/advanced/graphql.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/index.md` & `fastapi-0.99.1/docs/en/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/middleware.md` & `fastapi-0.99.1/docs/en/docs/advanced/middleware.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/nosql-databases.md` & `fastapi-0.99.1/docs/en/docs/advanced/nosql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/openapi-callbacks.md` & `fastapi-0.99.1/docs/en/docs/advanced/openapi-callbacks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/openapi-webhooks.md` & `fastapi-0.99.1/docs/en/docs/advanced/openapi-webhooks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/path-operation-advanced-configuration.md` & `fastapi-0.99.1/docs/en/docs/advanced/path-operation-advanced-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/response-change-status-code.md` & `fastapi-0.99.1/docs/en/docs/advanced/response-change-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/response-cookies.md` & `fastapi-0.99.1/docs/en/docs/advanced/response-cookies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/response-directly.md` & `fastapi-0.99.1/docs/en/docs/advanced/response-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/response-headers.md` & `fastapi-0.99.1/docs/en/docs/advanced/response-headers.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/settings.md` & `fastapi-0.99.1/docs/en/docs/advanced/settings.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/sql-databases-peewee.md` & `fastapi-0.99.1/docs/en/docs/advanced/sql-databases-peewee.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/sub-applications.md` & `fastapi-0.99.1/docs/en/docs/advanced/sub-applications.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/templates.md` & `fastapi-0.99.1/docs/en/docs/advanced/templates.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/testing-database.md` & `fastapi-0.99.1/docs/en/docs/advanced/testing-database.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/testing-dependencies.md` & `fastapi-0.99.1/docs/en/docs/advanced/testing-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/using-request-directly.md` & `fastapi-0.99.1/docs/en/docs/advanced/using-request-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/websockets.md` & `fastapi-0.99.1/docs/en/docs/advanced/websockets.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/wsgi.md` & `fastapi-0.99.1/docs/en/docs/advanced/wsgi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/security/http-basic-auth.md` & `fastapi-0.99.1/docs/en/docs/advanced/security/http-basic-auth.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/security/index.md` & `fastapi-0.99.1/docs/en/docs/advanced/security/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/advanced/security/oauth2-scopes.md` & `fastapi-0.99.1/docs/en/docs/advanced/security/oauth2-scopes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/css/custom.css` & `fastapi-0.99.1/docs/en/docs/css/custom.css`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/css/termynal.css` & `fastapi-0.99.1/docs/en/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/deployment/concepts.md` & `fastapi-0.99.1/docs/en/docs/deployment/concepts.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/deployment/deta.md` & `fastapi-0.99.1/docs/en/docs/deployment/deta.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/deployment/docker.md` & `fastapi-0.99.1/docs/en/docs/deployment/docker.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/deployment/https.md` & `fastapi-0.99.1/docs/en/docs/deployment/https.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/deployment/index.md` & `fastapi-0.99.1/docs/en/docs/deployment/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/deployment/manually.md` & `fastapi-0.99.1/docs/en/docs/deployment/manually.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/deployment/server-workers.md` & `fastapi-0.99.1/docs/en/docs/deployment/server-workers.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/deployment/versions.md` & `fastapi-0.99.1/docs/en/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/github-social-preview.png` & `fastapi-0.99.1/docs/en/docs/img/github-social-preview.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/github-social-preview.svg` & `fastapi-0.99.1/docs/en/docs/img/github-social-preview.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/icon-transparent-bg.png` & `fastapi-0.99.1/docs/en/docs/img/icon-transparent-bg.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/icon-white-bg.png` & `fastapi-0.99.1/docs/en/docs/img/icon-white-bg.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/icon-white.svg` & `fastapi-0.99.1/docs/en/docs/img/icon-white.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/logo-teal-vector.svg` & `fastapi-0.99.1/docs/en/docs/img/logo-teal-vector.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/logo-teal.svg` & `fastapi-0.99.1/docs/en/docs/img/logo-teal.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/pycharm-completion.png` & `fastapi-0.99.1/docs/en/docs/img/pycharm-completion.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/vscode-completion.png` & `fastapi-0.99.1/docs/en/docs/img/vscode-completion.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-01.png` & `fastapi-0.99.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-02.png` & `fastapi-0.99.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-03.png` & `fastapi-0.99.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-04.png` & `fastapi-0.99.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-05.png` & `fastapi-0.99.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-06.png` & `fastapi-0.99.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-06.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-07.png` & `fastapi-0.99.1/docs/en/docs/img/async/concurrent-burgers/concurrent-burgers-07.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-01.png` & `fastapi-0.99.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-02.png` & `fastapi-0.99.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-03.png` & `fastapi-0.99.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-04.png` & `fastapi-0.99.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-05.png` & `fastapi-0.99.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/async/parallel-burgers/parallel-burgers-06.png` & `fastapi-0.99.1/docs/en/docs/img/async/parallel-burgers/parallel-burgers-06.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/concepts/image01.png` & `fastapi-0.99.1/docs/en/docs/img/deployment/concepts/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/concepts/process-ram.drawio` & `fastapi-0.99.1/docs/en/docs/img/deployment/concepts/process-ram.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/concepts/process-ram.svg` & `fastapi-0.99.1/docs/en/docs/img/deployment/concepts/process-ram.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/deta/image01.png` & `fastapi-0.99.1/docs/en/docs/img/deployment/deta/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/deta/image02.png` & `fastapi-0.99.1/docs/en/docs/img/deployment/deta/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/deta/image03.png` & `fastapi-0.99.1/docs/en/docs/img/deployment/deta/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/deta/image04.png` & `fastapi-0.99.1/docs/en/docs/img/deployment/deta/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/deta/image05.png` & `fastapi-0.99.1/docs/en/docs/img/deployment/deta/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/deta/image06.png` & `fastapi-0.99.1/docs/en/docs/img/deployment/deta/image06.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/https/https.drawio` & `fastapi-0.99.1/docs/en/docs/img/deployment/https/https.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/https/https.svg` & `fastapi-0.99.1/docs/en/docs/img/deployment/https/https.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/https/https01.drawio` & `fastapi-0.99.1/docs/en/docs/img/deployment/https/https01.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/https/https01.svg` & `fastapi-0.99.1/docs/en/docs/img/deployment/https/https01.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/https/https02.drawio` & `fastapi-0.99.1/docs/en/docs/img/deployment/https/https02.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/https/https02.svg` & `fastapi-0.99.1/docs/en/docs/img/deployment/https/https02.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/https/https03.drawio` & `fastapi-0.99.1/docs/en/docs/img/deployment/https/https03.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/https/https03.svg` & `fastapi-0.99.1/docs/en/docs/img/deployment/https/https03.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/https/https04.drawio` & `fastapi-0.99.1/docs/en/docs/img/deployment/https/https04.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/https/https04.svg` & `fastapi-0.99.1/docs/en/docs/img/deployment/https/https04.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/https/https05.drawio` & `fastapi-0.99.1/docs/en/docs/img/deployment/https/https05.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/https/https05.svg` & `fastapi-0.99.1/docs/en/docs/img/deployment/https/https05.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/https/https06.drawio` & `fastapi-0.99.1/docs/en/docs/img/deployment/https/https06.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/https/https06.svg` & `fastapi-0.99.1/docs/en/docs/img/deployment/https/https06.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/https/https07.drawio` & `fastapi-0.99.1/docs/en/docs/img/deployment/https/https07.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/https/https07.svg` & `fastapi-0.99.1/docs/en/docs/img/deployment/https/https07.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/https/https08.drawio` & `fastapi-0.99.1/docs/en/docs/img/deployment/https/https08.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/deployment/https/https08.svg` & `fastapi-0.99.1/docs/en/docs/img/deployment/https/https08.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/index/index-01-swagger-ui-simple.png` & `fastapi-0.99.1/docs/en/docs/img/index/index-01-swagger-ui-simple.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/index/index-02-redoc-simple.png` & `fastapi-0.99.1/docs/en/docs/img/index/index-02-redoc-simple.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/index/index-03-swagger-02.png` & `fastapi-0.99.1/docs/en/docs/img/index/index-03-swagger-02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/index/index-04-swagger-03.png` & `fastapi-0.99.1/docs/en/docs/img/index/index-04-swagger-03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/index/index-05-swagger-04.png` & `fastapi-0.99.1/docs/en/docs/img/index/index-05-swagger-04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/index/index-06-redoc-02.png` & `fastapi-0.99.1/docs/en/docs/img/index/index-06-redoc-02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/logo-margin/logo-teal-vector.svg` & `fastapi-0.99.1/docs/en/docs/img/logo-margin/logo-teal-vector.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/logo-margin/logo-teal.png` & `fastapi-0.99.1/docs/en/docs/img/logo-margin/logo-teal.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/logo-margin/logo-teal.svg` & `fastapi-0.99.1/docs/en/docs/img/logo-margin/logo-teal.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/logo-margin/logo-white-bg.png` & `fastapi-0.99.1/docs/en/docs/img/logo-margin/logo-white-bg.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/python-types/image01.png` & `fastapi-0.99.1/docs/en/docs/img/python-types/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/python-types/image02.png` & `fastapi-0.99.1/docs/en/docs/img/python-types/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/python-types/image03.png` & `fastapi-0.99.1/docs/en/docs/img/python-types/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/python-types/image04.png` & `fastapi-0.99.1/docs/en/docs/img/python-types/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/python-types/image05.png` & `fastapi-0.99.1/docs/en/docs/img/python-types/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/python-types/image06.png` & `fastapi-0.99.1/docs/en/docs/img/python-types/image06.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/budget-insight.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/budget-insight.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/calmcode.jpg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/calmcode.jpg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/classiq-banner.png` & `fastapi-0.99.1/docs/en/docs/img/sponsors/classiq-banner.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/classiq.png` & `fastapi-0.99.1/docs/en/docs/img/sponsors/classiq.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/cryptapi-banner.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/cryptapi-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/cryptapi.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/cryptapi.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/databento.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/databento.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/deta-banner.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/deta-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/deta.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/deta.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/docarray-top-banner.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/docarray-top-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/docarray.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/docarray.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/doist-banner.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/doist-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/doist.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/doist.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/dropbase-banner.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/dropbase-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/dropbase.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/dropbase.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/exoflare.png` & `fastapi-0.99.1/docs/en/docs/img/sponsors/exoflare.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.png` & `fastapi-0.99.1/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/fastapi-course-bundle-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/flint.png` & `fastapi-0.99.1/docs/en/docs/img/sponsors/flint.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/haystack-fastapi.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/haystack-fastapi.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/imgwhale-banner.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/imgwhale-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/imgwhale.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/imgwhale.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/ines-course.jpg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/ines-course.jpg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/investsuite.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/investsuite.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/jina-ai-banner.png` & `fastapi-0.99.1/docs/en/docs/img/sponsors/jina-ai-banner.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/jina-ai.png` & `fastapi-0.99.1/docs/en/docs/img/sponsors/jina-ai.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/jina-banner.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/jina-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/jina-top-banner.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/jina-top-banner.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/jina.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/jina.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/jina2.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/jina2.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/platform-sh-banner.png` & `fastapi-0.99.1/docs/en/docs/img/sponsors/platform-sh-banner.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/platform-sh.png` & `fastapi-0.99.1/docs/en/docs/img/sponsors/platform-sh.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/powens.png` & `fastapi-0.99.1/docs/en/docs/img/sponsors/powens.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/striveworks-banner.png` & `fastapi-0.99.1/docs/en/docs/img/sponsors/striveworks-banner.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/striveworks.png` & `fastapi-0.99.1/docs/en/docs/img/sponsors/striveworks.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/striveworks2.png` & `fastapi-0.99.1/docs/en/docs/img/sponsors/striveworks2.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/svix.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/svix.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/talkpython.png` & `fastapi-0.99.1/docs/en/docs/img/sponsors/talkpython.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/testdriven.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/testdriven.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/vimso.png` & `fastapi-0.99.1/docs/en/docs/img/sponsors/vimso.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/sponsors/wetransfer.svg` & `fastapi-0.99.1/docs/en/docs/img/sponsors/wetransfer.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/additional-responses/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/additional-responses/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/async-sql-databases/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/async-sql-databases/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/behind-a-proxy/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/behind-a-proxy/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/behind-a-proxy/image02.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/behind-a-proxy/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/behind-a-proxy/image03.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/behind-a-proxy/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/bigger-applications/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/bigger-applications/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/bigger-applications/package.drawio` & `fastapi-0.99.1/docs/en/docs/img/tutorial/bigger-applications/package.drawio`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/bigger-applications/package.svg` & `fastapi-0.99.1/docs/en/docs/img/tutorial/bigger-applications/package.svg`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/body/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/body/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/body/image02.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/body/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/body/image03.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/body/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/body/image04.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/body/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/body/image05.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/body/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/body-fields/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/body-fields/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/body-fields/image02.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/body-fields/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/body-nested-models/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/body-nested-models/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/custom-response/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/custom-response/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/dataclasses/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/dataclasses/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/debugging/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/debugging/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/debugging/image02.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/debugging/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/dependencies/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/dependencies/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/dependencies/image02.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/dependencies/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/extending-openapi/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/extending-openapi/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/extending-openapi/image02.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/extending-openapi/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/extending-openapi/image03.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/extending-openapi/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/extending-openapi/image04.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/extending-openapi/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/generate-clients/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/generate-clients/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/generate-clients/image02.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/generate-clients/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/generate-clients/image03.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/generate-clients/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/generate-clients/image04.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/generate-clients/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/generate-clients/image05.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/generate-clients/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/generate-clients/image06.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/generate-clients/image06.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/generate-clients/image07.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/generate-clients/image07.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/generate-clients/image08.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/generate-clients/image08.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/graphql/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/graphql/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/metadata/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/metadata/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/metadata/image02.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/metadata/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/openapi-callbacks/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/openapi-callbacks/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/openapi-webhooks/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/openapi-webhooks/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/path-operation-advanced-configuration/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/path-operation-advanced-configuration/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/path-operation-configuration/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/path-operation-configuration/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/path-operation-configuration/image02.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/path-operation-configuration/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/path-operation-configuration/image03.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/path-operation-configuration/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/path-operation-configuration/image04.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/path-operation-configuration/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/path-operation-configuration/image05.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/path-operation-configuration/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/path-params/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/path-params/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/path-params/image02.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/path-params/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/path-params/image03.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/path-params/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/query-params-str-validations/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/query-params-str-validations/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/query-params-str-validations/image02.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/query-params-str-validations/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/response-model/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/response-model/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/response-model/image02.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/response-model/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/response-status-code/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/response-status-code/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/response-status-code/image02.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/response-status-code/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/security/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/security/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/security/image02.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/security/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/security/image03.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/security/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/security/image04.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/security/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/security/image05.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/security/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/security/image06.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/security/image06.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/security/image07.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/security/image07.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/security/image08.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/security/image08.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/security/image09.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/security/image09.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/security/image10.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/security/image10.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/security/image11.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/security/image11.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/security/image12.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/security/image12.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/sql-databases/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/sql-databases/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/sql-databases/image02.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/sql-databases/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/sub-applications/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/sub-applications/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/sub-applications/image02.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/sub-applications/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/websockets/image01.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/websockets/image01.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/websockets/image02.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/websockets/image02.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/websockets/image03.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/websockets/image03.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/websockets/image04.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/websockets/image04.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/img/tutorial/websockets/image05.png` & `fastapi-0.99.1/docs/en/docs/img/tutorial/websockets/image05.png`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/js/custom.js` & `fastapi-0.99.1/docs/en/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/js/termynal.js` & `fastapi-0.99.1/docs/en/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/background-tasks.md` & `fastapi-0.99.1/docs/en/docs/tutorial/background-tasks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/bigger-applications.md` & `fastapi-0.99.1/docs/en/docs/tutorial/bigger-applications.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/body-fields.md` & `fastapi-0.99.1/docs/en/docs/tutorial/body-fields.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/body-multiple-params.md` & `fastapi-0.99.1/docs/en/docs/tutorial/body-multiple-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/body-nested-models.md` & `fastapi-0.99.1/docs/en/docs/tutorial/body-nested-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/body-updates.md` & `fastapi-0.99.1/docs/en/docs/tutorial/body-updates.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/body.md` & `fastapi-0.99.1/docs/en/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/cookie-params.md` & `fastapi-0.99.1/docs/en/docs/tutorial/cookie-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/cors.md` & `fastapi-0.99.1/docs/en/docs/tutorial/cors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/debugging.md` & `fastapi-0.99.1/docs/en/docs/tutorial/debugging.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/encoder.md` & `fastapi-0.99.1/docs/en/docs/tutorial/encoder.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/extra-data-types.md` & `fastapi-0.99.1/docs/en/docs/tutorial/extra-data-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/extra-models.md` & `fastapi-0.99.1/docs/en/docs/tutorial/extra-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/first-steps.md` & `fastapi-0.99.1/docs/en/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/handling-errors.md` & `fastapi-0.99.1/docs/en/docs/tutorial/handling-errors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/header-params.md` & `fastapi-0.99.1/docs/en/docs/tutorial/header-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/index.md` & `fastapi-0.99.1/docs/en/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/metadata.md` & `fastapi-0.99.1/docs/en/docs/tutorial/metadata.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/middleware.md` & `fastapi-0.99.1/docs/en/docs/tutorial/middleware.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/path-operation-configuration.md` & `fastapi-0.99.1/docs/en/docs/tutorial/path-operation-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/path-params-numeric-validations.md` & `fastapi-0.99.1/docs/en/docs/tutorial/path-params-numeric-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/path-params.md` & `fastapi-0.99.1/docs/en/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/query-params-str-validations.md` & `fastapi-0.99.1/docs/en/docs/tutorial/query-params-str-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/query-params.md` & `fastapi-0.99.1/docs/en/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/request-files.md` & `fastapi-0.99.1/docs/en/docs/tutorial/request-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/request-forms-and-files.md` & `fastapi-0.99.1/docs/en/docs/tutorial/request-forms-and-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/request-forms.md` & `fastapi-0.99.1/docs/en/docs/tutorial/request-forms.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/response-model.md` & `fastapi-0.99.1/docs/en/docs/tutorial/response-model.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/response-status-code.md` & `fastapi-0.99.1/docs/en/docs/tutorial/response-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/schema-extra-example.md` & `fastapi-0.99.1/docs/en/docs/tutorial/schema-extra-example.md`

 * *Files 1% similar despite different names*

```diff
@@ -112,45 +112,45 @@
 
 ### `Body` with multiple `examples`
 
 You can of course also pass multiple `examples`:
 
 === "Python 3.10+"
 
-    ```Python hl_lines="23-49"
+    ```Python hl_lines="23-38"
     {!> ../../../docs_src/schema_extra_example/tutorial004_an_py310.py!}
     ```
 
 === "Python 3.9+"
 
-    ```Python hl_lines="23-49"
+    ```Python hl_lines="23-38"
     {!> ../../../docs_src/schema_extra_example/tutorial004_an_py39.py!}
     ```
 
 === "Python 3.6+"
 
-    ```Python hl_lines="24-50"
+    ```Python hl_lines="24-39"
     {!> ../../../docs_src/schema_extra_example/tutorial004_an.py!}
     ```
 
 === "Python 3.10+ non-Annotated"
 
     !!! tip
         Prefer to use the `Annotated` version if possible.
 
-    ```Python hl_lines="19-45"
+    ```Python hl_lines="19-34"
     {!> ../../../docs_src/schema_extra_example/tutorial004_py310.py!}
     ```
 
 === "Python 3.6+ non-Annotated"
 
     !!! tip
         Prefer to use the `Annotated` version if possible.
 
-    ```Python hl_lines="21-47"
+    ```Python hl_lines="21-36"
     {!> ../../../docs_src/schema_extra_example/tutorial004.py!}
     ```
 
 ### Examples in the docs UI
 
 With `examples` added to `Body()` the `/docs` would look like:
```

#### html2text {}

```diff
@@ -32,23 +32,23 @@
 ```Python hl_lines="18-25" {!> ../../../docs_src/schema_extra_example/
 tutorial003_py310.py!} ``` === "Python 3.6+ non-Annotated" !!! tip Prefer to
 use the `Annotated` version if possible. ```Python hl_lines="20-27" {!>
 ../../../docs_src/schema_extra_example/tutorial003.py!} ``` ### Example in the
 docs UI With any of the methods above it would look like this in the `/docs`:
 [/img/tutorial/body-fields/image01.png] ### `Body` with multiple `examples` You
 can of course also pass multiple `examples`: === "Python 3.10+" ```Python
-hl_lines="23-49" {!> ../../../docs_src/schema_extra_example/
-tutorial004_an_py310.py!} ``` === "Python 3.9+" ```Python hl_lines="23-49" {!>
+hl_lines="23-38" {!> ../../../docs_src/schema_extra_example/
+tutorial004_an_py310.py!} ``` === "Python 3.9+" ```Python hl_lines="23-38" {!>
 ../../../docs_src/schema_extra_example/tutorial004_an_py39.py!} ``` === "Python
-3.6+" ```Python hl_lines="24-50" {!> ../../../docs_src/schema_extra_example/
+3.6+" ```Python hl_lines="24-39" {!> ../../../docs_src/schema_extra_example/
 tutorial004_an.py!} ``` === "Python 3.10+ non-Annotated" !!! tip Prefer to use
-the `Annotated` version if possible. ```Python hl_lines="19-45" {!> ../../../
+the `Annotated` version if possible. ```Python hl_lines="19-34" {!> ../../../
 docs_src/schema_extra_example/tutorial004_py310.py!} ``` === "Python 3.6+ non-
 Annotated" !!! tip Prefer to use the `Annotated` version if possible. ```Python
-hl_lines="21-47" {!> ../../../docs_src/schema_extra_example/tutorial004.py!}
+hl_lines="21-36" {!> ../../../docs_src/schema_extra_example/tutorial004.py!}
 ``` ### Examples in the docs UI With `examples` added to `Body()` the `/docs`
 would look like: [/img/tutorial/body-fields/image02.png] ## Technical Details
 !!! tip If you are already using **FastAPI** version **0.99.0 or above**, you
 can probably **skip** these details. They are more relevant for older versions,
 before OpenAPI 3.1.0 was available. You can consider this a brief OpenAPI and
 JSON Schema **history lesson**. ð¤ !!! warning These are very technical
 details about the standards **JSON Schema** and **OpenAPI**. If the ideas above
```

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/sql-databases.md` & `fastapi-0.99.1/docs/en/docs/tutorial/sql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/static-files.md` & `fastapi-0.99.1/docs/en/docs/tutorial/static-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/testing.md` & `fastapi-0.99.1/docs/en/docs/tutorial/testing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/dependencies/classes-as-dependencies.md` & `fastapi-0.99.1/docs/en/docs/tutorial/dependencies/classes-as-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md` & `fastapi-0.99.1/docs/en/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/dependencies/dependencies-with-yield.md` & `fastapi-0.99.1/docs/en/docs/tutorial/dependencies/dependencies-with-yield.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/dependencies/global-dependencies.md` & `fastapi-0.99.1/docs/en/docs/tutorial/dependencies/global-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/dependencies/index.md` & `fastapi-0.99.1/docs/en/docs/tutorial/dependencies/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/dependencies/sub-dependencies.md` & `fastapi-0.99.1/docs/en/docs/tutorial/dependencies/sub-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/security/first-steps.md` & `fastapi-0.99.1/docs/en/docs/tutorial/security/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/security/get-current-user.md` & `fastapi-0.99.1/docs/en/docs/tutorial/security/get-current-user.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/security/index.md` & `fastapi-0.99.1/docs/en/docs/tutorial/security/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/security/oauth2-jwt.md` & `fastapi-0.99.1/docs/en/docs/tutorial/security/oauth2-jwt.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/docs/tutorial/security/simple-oauth2.md` & `fastapi-0.99.1/docs/en/docs/tutorial/security/simple-oauth2.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/layouts/custom.yml` & `fastapi-0.99.1/docs/en/layouts/custom.yml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/en/overrides/main.html` & `fastapi-0.99.1/docs/en/overrides/main.html`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/es/docs/async.md` & `fastapi-0.99.1/docs/es/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/es/docs/features.md` & `fastapi-0.99.1/docs/es/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/es/docs/index.md` & `fastapi-0.99.1/docs/es/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/es/docs/python-types.md` & `fastapi-0.99.1/docs/es/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/es/docs/advanced/additional-status-codes.md` & `fastapi-0.99.1/docs/es/docs/advanced/additional-status-codes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/es/docs/advanced/index.md` & `fastapi-0.99.1/docs/es/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/es/docs/advanced/path-operation-advanced-configuration.md` & `fastapi-0.99.1/docs/es/docs/advanced/path-operation-advanced-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/es/docs/advanced/response-directly.md` & `fastapi-0.99.1/docs/es/docs/advanced/response-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/es/docs/tutorial/first-steps.md` & `fastapi-0.99.1/docs/es/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/es/docs/tutorial/index.md` & `fastapi-0.99.1/docs/es/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/es/docs/tutorial/path-params.md` & `fastapi-0.99.1/docs/es/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/es/docs/tutorial/query-params.md` & `fastapi-0.99.1/docs/es/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fa/docs/index.md` & `fastapi-0.99.1/docs/fa/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fa/docs/advanced/sub-applications.md` & `fastapi-0.99.1/docs/fa/docs/advanced/sub-applications.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/alternatives.md` & `fastapi-0.99.1/docs/fr/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/async.md` & `fastapi-0.99.1/docs/fr/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/external-links.md` & `fastapi-0.99.1/docs/fr/docs/external-links.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/fastapi-people.md` & `fastapi-0.99.1/docs/fr/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/features.md` & `fastapi-0.99.1/docs/fr/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/help-fastapi.md` & `fastapi-0.99.1/docs/fr/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/history-design-future.md` & `fastapi-0.99.1/docs/fr/docs/history-design-future.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/index.md` & `fastapi-0.99.1/docs/fr/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/project-generation.md` & `fastapi-0.99.1/docs/fr/docs/project-generation.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/python-types.md` & `fastapi-0.99.1/docs/fr/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/advanced/additional-responses.md` & `fastapi-0.99.1/docs/fr/docs/advanced/additional-responses.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/advanced/additional-status-codes.md` & `fastapi-0.99.1/docs/fr/docs/advanced/additional-status-codes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/advanced/index.md` & `fastapi-0.99.1/docs/fr/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/advanced/path-operation-advanced-configuration.md` & `fastapi-0.99.1/docs/fr/docs/advanced/path-operation-advanced-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/advanced/response-directly.md` & `fastapi-0.99.1/docs/fr/docs/advanced/response-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/deployment/deta.md` & `fastapi-0.99.1/docs/fr/docs/deployment/deta.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/deployment/docker.md` & `fastapi-0.99.1/docs/fr/docs/deployment/docker.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/deployment/https.md` & `fastapi-0.99.1/docs/fr/docs/deployment/https.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/deployment/index.md` & `fastapi-0.99.1/docs/fr/docs/deployment/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/deployment/manually.md` & `fastapi-0.99.1/docs/fr/docs/deployment/manually.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/deployment/versions.md` & `fastapi-0.99.1/docs/fr/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/tutorial/background-tasks.md` & `fastapi-0.99.1/docs/fr/docs/tutorial/background-tasks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/tutorial/body.md` & `fastapi-0.99.1/docs/fr/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/tutorial/debugging.md` & `fastapi-0.99.1/docs/fr/docs/tutorial/debugging.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/tutorial/first-steps.md` & `fastapi-0.99.1/docs/fr/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/tutorial/path-params.md` & `fastapi-0.99.1/docs/fr/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/fr/docs/tutorial/query-params.md` & `fastapi-0.99.1/docs/fr/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/he/docs/index.md` & `fastapi-0.99.1/docs/he/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/id/docs/tutorial/index.md` & `fastapi-0.99.1/docs/id/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/alternatives.md` & `fastapi-0.99.1/docs/ja/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/async.md` & `fastapi-0.99.1/docs/ja/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/benchmarks.md` & `fastapi-0.99.1/docs/ja/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/contributing.md` & `fastapi-0.99.1/docs/ja/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/external-links.md` & `fastapi-0.99.1/docs/ja/docs/external-links.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/fastapi-people.md` & `fastapi-0.99.1/docs/ja/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/features.md` & `fastapi-0.99.1/docs/ja/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/help-fastapi.md` & `fastapi-0.99.1/docs/ja/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/history-design-future.md` & `fastapi-0.99.1/docs/ja/docs/history-design-future.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/index.md` & `fastapi-0.99.1/docs/ja/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/project-generation.md` & `fastapi-0.99.1/docs/ja/docs/project-generation.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/advanced/additional-status-codes.md` & `fastapi-0.99.1/docs/ja/docs/advanced/additional-status-codes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/advanced/conditional-openapi.md` & `fastapi-0.99.1/docs/ja/docs/advanced/conditional-openapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/advanced/custom-response.md` & `fastapi-0.99.1/docs/ja/docs/advanced/custom-response.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/advanced/index.md` & `fastapi-0.99.1/docs/ja/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/advanced/nosql-databases.md` & `fastapi-0.99.1/docs/ja/docs/advanced/nosql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/advanced/path-operation-advanced-configuration.md` & `fastapi-0.99.1/docs/ja/docs/advanced/path-operation-advanced-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/advanced/response-directly.md` & `fastapi-0.99.1/docs/ja/docs/advanced/response-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/advanced/websockets.md` & `fastapi-0.99.1/docs/ja/docs/advanced/websockets.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/deployment/deta.md` & `fastapi-0.99.1/docs/ja/docs/deployment/deta.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/deployment/docker.md` & `fastapi-0.99.1/docs/ja/docs/deployment/docker.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/deployment/manually.md` & `fastapi-0.99.1/docs/ja/docs/deployment/manually.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/deployment/versions.md` & `fastapi-0.99.1/docs/ja/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/tutorial/body-updates.md` & `fastapi-0.99.1/docs/ja/docs/tutorial/body-updates.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/tutorial/body.md` & `fastapi-0.99.1/docs/ja/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/tutorial/cookie-params.md` & `fastapi-0.99.1/docs/ja/docs/tutorial/cookie-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/tutorial/cors.md` & `fastapi-0.99.1/docs/ja/docs/tutorial/cors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/tutorial/debugging.md` & `fastapi-0.99.1/docs/ja/docs/tutorial/debugging.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/tutorial/first-steps.md` & `fastapi-0.99.1/docs/ja/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/tutorial/header-params.md` & `fastapi-0.99.1/docs/ja/docs/tutorial/header-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/tutorial/index.md` & `fastapi-0.99.1/docs/ja/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/tutorial/middleware.md` & `fastapi-0.99.1/docs/ja/docs/tutorial/middleware.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/tutorial/path-params.md` & `fastapi-0.99.1/docs/ja/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/tutorial/query-params-str-validations.md` & `fastapi-0.99.1/docs/ja/docs/tutorial/query-params-str-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/tutorial/query-params.md` & `fastapi-0.99.1/docs/ja/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/tutorial/request-forms.md` & `fastapi-0.99.1/docs/ja/docs/tutorial/request-forms.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/tutorial/static-files.md` & `fastapi-0.99.1/docs/ja/docs/tutorial/static-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/tutorial/testing.md` & `fastapi-0.99.1/docs/ja/docs/tutorial/testing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/tutorial/security/first-steps.md` & `fastapi-0.99.1/docs/ja/docs/tutorial/security/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ja/docs/tutorial/security/oauth2-jwt.md` & `fastapi-0.99.1/docs/ja/docs/tutorial/security/oauth2-jwt.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ko/docs/index.md` & `fastapi-0.99.1/docs/ko/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ko/docs/deployment/versions.md` & `fastapi-0.99.1/docs/ko/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ko/docs/tutorial/cors.md` & `fastapi-0.99.1/docs/ko/docs/tutorial/cors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ko/docs/tutorial/encoder.md` & `fastapi-0.99.1/docs/ko/docs/tutorial/encoder.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ko/docs/tutorial/first-steps.md` & `fastapi-0.99.1/docs/ko/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ko/docs/tutorial/header-params.md` & `fastapi-0.99.1/docs/ko/docs/tutorial/header-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ko/docs/tutorial/index.md` & `fastapi-0.99.1/docs/ko/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ko/docs/tutorial/path-params-numeric-validations.md` & `fastapi-0.99.1/docs/ko/docs/tutorial/path-params-numeric-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ko/docs/tutorial/path-params.md` & `fastapi-0.99.1/docs/ko/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ko/docs/tutorial/query-params.md` & `fastapi-0.99.1/docs/ko/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ko/docs/tutorial/request-files.md` & `fastapi-0.99.1/docs/ko/docs/tutorial/request-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ko/docs/tutorial/request-forms-and-files.md` & `fastapi-0.99.1/docs/ko/docs/tutorial/request-forms-and-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ko/docs/tutorial/response-status-code.md` & `fastapi-0.99.1/docs/ko/docs/tutorial/response-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ko/docs/tutorial/dependencies/classes-as-dependencies.md` & `fastapi-0.99.1/docs/ko/docs/tutorial/dependencies/classes-as-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pl/docs/features.md` & `fastapi-0.99.1/docs/pl/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pl/docs/index.md` & `fastapi-0.99.1/docs/pl/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pl/docs/tutorial/first-steps.md` & `fastapi-0.99.1/docs/pl/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pl/docs/tutorial/index.md` & `fastapi-0.99.1/docs/pl/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/alternatives.md` & `fastapi-0.99.1/docs/pt/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/async.md` & `fastapi-0.99.1/docs/pt/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/benchmarks.md` & `fastapi-0.99.1/docs/pt/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/contributing.md` & `fastapi-0.99.1/docs/pt/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/deployment.md` & `fastapi-0.99.1/docs/pt/docs/deployment.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/external-links.md` & `fastapi-0.99.1/docs/pt/docs/external-links.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/fastapi-people.md` & `fastapi-0.99.1/docs/pt/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/features.md` & `fastapi-0.99.1/docs/pt/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/help-fastapi.md` & `fastapi-0.99.1/docs/pt/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/history-design-future.md` & `fastapi-0.99.1/docs/pt/docs/history-design-future.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/index.md` & `fastapi-0.99.1/docs/pt/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/project-generation.md` & `fastapi-0.99.1/docs/pt/docs/project-generation.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/python-types.md` & `fastapi-0.99.1/docs/pt/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/advanced/events.md` & `fastapi-0.99.1/docs/pt/docs/advanced/events.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/advanced/index.md` & `fastapi-0.99.1/docs/pt/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/deployment/deta.md` & `fastapi-0.99.1/docs/pt/docs/deployment/deta.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/deployment/docker.md` & `fastapi-0.99.1/docs/pt/docs/deployment/docker.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/deployment/https.md` & `fastapi-0.99.1/docs/pt/docs/deployment/https.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/deployment/versions.md` & `fastapi-0.99.1/docs/pt/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/background-tasks.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/background-tasks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/body-fields.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/body-fields.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/body-multiple-params.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/body-multiple-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/body-nested-models.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/body-nested-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/body.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/cookie-params.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/cookie-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/encoder.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/encoder.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/extra-data-types.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/extra-data-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/extra-models.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/extra-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/first-steps.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/handling-errors.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/handling-errors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/header-params.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/header-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/index.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/path-operation-configuration.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/path-operation-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/path-params-numeric-validations.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/path-params-numeric-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/path-params.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/query-params-str-validations.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/query-params-str-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/query-params.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/request-forms-and-files.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/request-forms-and-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/request-forms.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/request-forms.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/response-status-code.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/response-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/static-files.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/static-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/security/first-steps.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/security/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/pt/docs/tutorial/security/index.md` & `fastapi-0.99.1/docs/pt/docs/tutorial/security/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/alternatives.md` & `fastapi-0.99.1/docs/ru/docs/alternatives.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/async.md` & `fastapi-0.99.1/docs/ru/docs/async.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/benchmarks.md` & `fastapi-0.99.1/docs/ru/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/contributing.md` & `fastapi-0.99.1/docs/ru/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/external-links.md` & `fastapi-0.99.1/docs/ru/docs/external-links.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/fastapi-people.md` & `fastapi-0.99.1/docs/ru/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/features.md` & `fastapi-0.99.1/docs/ru/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/help-fastapi.md` & `fastapi-0.99.1/docs/ru/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/history-design-future.md` & `fastapi-0.99.1/docs/ru/docs/history-design-future.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/index.md` & `fastapi-0.99.1/docs/ru/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/project-generation.md` & `fastapi-0.99.1/docs/ru/docs/project-generation.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/python-types.md` & `fastapi-0.99.1/docs/ru/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/deployment/concepts.md` & `fastapi-0.99.1/docs/ru/docs/deployment/concepts.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/deployment/https.md` & `fastapi-0.99.1/docs/ru/docs/deployment/https.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/deployment/index.md` & `fastapi-0.99.1/docs/ru/docs/deployment/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/deployment/manually.md` & `fastapi-0.99.1/docs/ru/docs/deployment/manually.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/deployment/versions.md` & `fastapi-0.99.1/docs/ru/docs/deployment/versions.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/background-tasks.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/background-tasks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/body-fields.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/body-fields.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/body-multiple-params.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/body-multiple-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/body-nested-models.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/body-nested-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/body.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/cookie-params.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/cookie-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/cors.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/cors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/debugging.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/debugging.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/extra-data-types.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/extra-data-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/extra-models.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/extra-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/first-steps.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/index.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/metadata.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/metadata.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/path-operation-configuration.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/path-operation-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/path-params-numeric-validations.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/path-params-numeric-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/path-params.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/query-params-str-validations.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/query-params-str-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/query-params.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/response-model.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/response-model.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/response-status-code.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/response-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/schema-extra-example.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/schema-extra-example.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/static-files.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/static-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/ru/docs/tutorial/testing.md` & `fastapi-0.99.1/docs/ru/docs/tutorial/testing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/tr/docs/benchmarks.md` & `fastapi-0.99.1/docs/tr/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/tr/docs/fastapi-people.md` & `fastapi-0.99.1/docs/tr/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/tr/docs/features.md` & `fastapi-0.99.1/docs/tr/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/tr/docs/index.md` & `fastapi-0.99.1/docs/tr/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/tr/docs/python-types.md` & `fastapi-0.99.1/docs/tr/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/tr/docs/tutorial/first_steps.md` & `fastapi-0.99.1/docs/tr/docs/tutorial/first_steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/benchmarks.md` & `fastapi-0.99.1/docs/zh/docs/benchmarks.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/contributing.md` & `fastapi-0.99.1/docs/zh/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/fastapi-people.md` & `fastapi-0.99.1/docs/zh/docs/fastapi-people.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/features.md` & `fastapi-0.99.1/docs/zh/docs/features.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/help-fastapi.md` & `fastapi-0.99.1/docs/zh/docs/help-fastapi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/index.md` & `fastapi-0.99.1/docs/zh/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/python-types.md` & `fastapi-0.99.1/docs/zh/docs/python-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/advanced/additional-status-codes.md` & `fastapi-0.99.1/docs/zh/docs/advanced/additional-status-codes.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/advanced/custom-response.md` & `fastapi-0.99.1/docs/zh/docs/advanced/custom-response.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/advanced/index.md` & `fastapi-0.99.1/docs/zh/docs/advanced/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/advanced/path-operation-advanced-configuration.md` & `fastapi-0.99.1/docs/zh/docs/advanced/path-operation-advanced-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/advanced/response-change-status-code.md` & `fastapi-0.99.1/docs/zh/docs/advanced/response-change-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/advanced/response-cookies.md` & `fastapi-0.99.1/docs/zh/docs/advanced/response-cookies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/advanced/response-directly.md` & `fastapi-0.99.1/docs/zh/docs/advanced/response-directly.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/advanced/response-headers.md` & `fastapi-0.99.1/docs/zh/docs/advanced/response-headers.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/advanced/settings.md` & `fastapi-0.99.1/docs/zh/docs/advanced/settings.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/advanced/websockets.md` & `fastapi-0.99.1/docs/zh/docs/advanced/websockets.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/advanced/wsgi.md` & `fastapi-0.99.1/docs/zh/docs/advanced/wsgi.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/advanced/security/index.md` & `fastapi-0.99.1/docs/zh/docs/advanced/security/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/bigger-applications.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/bigger-applications.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/body-fields.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/body-fields.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/body-multiple-params.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/body-multiple-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/body-nested-models.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/body-nested-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/body-updates.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/body-updates.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/body.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/body.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/cookie-params.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/cookie-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/cors.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/cors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/debugging.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/debugging.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/encoder.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/encoder.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/extra-data-types.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/extra-data-types.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/extra-models.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/extra-models.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/first-steps.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/handling-errors.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/handling-errors.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/header-params.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/header-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/index.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/metadata.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/metadata.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/middleware.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/middleware.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/path-operation-configuration.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/path-operation-configuration.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/path-params-numeric-validations.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/path-params-numeric-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/path-params.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/path-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/query-params-str-validations.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/query-params-str-validations.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/query-params.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/query-params.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/request-files.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/request-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/request-forms-and-files.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/request-forms-and-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/request-forms.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/request-forms.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/response-model.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/response-model.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/response-status-code.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/response-status-code.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/schema-extra-example.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/schema-extra-example.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/sql-databases.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/sql-databases.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/static-files.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/static-files.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/testing.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/testing.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/dependencies/classes-as-dependencies.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/dependencies/classes-as-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/dependencies/dependencies-in-path-operation-decorators.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/dependencies/global-dependencies.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/dependencies/global-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/dependencies/index.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/dependencies/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/dependencies/sub-dependencies.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/dependencies/sub-dependencies.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/security/first-steps.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/security/first-steps.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/security/get-current-user.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/security/get-current-user.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/security/index.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/security/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/security/oauth2-jwt.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/security/oauth2-jwt.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs/zh/docs/tutorial/security/simple-oauth2.md` & `fastapi-0.99.1/docs/zh/docs/tutorial/security/simple-oauth2.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/additional_responses/tutorial002.py` & `fastapi-0.99.1/docs_src/additional_responses/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/additional_responses/tutorial003.py` & `fastapi-0.99.1/docs_src/additional_responses/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/additional_responses/tutorial004.py` & `fastapi-0.99.1/docs_src/additional_responses/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/additional_status_codes/tutorial001.py` & `fastapi-0.99.1/docs_src/additional_status_codes/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/additional_status_codes/tutorial001_an.py` & `fastapi-0.99.1/docs_src/additional_status_codes/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/additional_status_codes/tutorial001_an_py310.py` & `fastapi-0.99.1/docs_src/additional_status_codes/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/additional_status_codes/tutorial001_an_py39.py` & `fastapi-0.99.1/docs_src/additional_status_codes/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/additional_status_codes/tutorial001_py310.py` & `fastapi-0.99.1/docs_src/additional_status_codes/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/app_testing/tutorial002.py` & `fastapi-0.99.1/docs_src/app_testing/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/app_testing/tutorial003.py` & `fastapi-0.99.1/docs_src/app_testing/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/app_testing/app_b/main.py` & `fastapi-0.99.1/docs_src/app_testing/app_b/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/app_testing/app_b/test_main.py` & `fastapi-0.99.1/docs_src/app_testing/app_b/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/app_testing/app_b_an/main.py` & `fastapi-0.99.1/docs_src/app_testing/app_b_an/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/app_testing/app_b_an/test_main.py` & `fastapi-0.99.1/docs_src/app_testing/app_b_an/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/app_testing/app_b_an_py310/main.py` & `fastapi-0.99.1/docs_src/app_testing/app_b_an_py310/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/app_testing/app_b_an_py310/test_main.py` & `fastapi-0.99.1/docs_src/app_testing/app_b_an_py310/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/app_testing/app_b_an_py39/main.py` & `fastapi-0.99.1/docs_src/app_testing/app_b_an_py39/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/app_testing/app_b_an_py39/test_main.py` & `fastapi-0.99.1/docs_src/app_testing/app_b_an_py39/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/app_testing/app_b_py310/main.py` & `fastapi-0.99.1/docs_src/app_testing/app_b_py310/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/app_testing/app_b_py310/test_main.py` & `fastapi-0.99.1/docs_src/app_testing/app_b_py310/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/async_sql_databases/tutorial001.py` & `fastapi-0.99.1/docs_src/async_sql_databases/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/background_tasks/tutorial001.py` & `fastapi-0.99.1/docs_src/background_tasks/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/background_tasks/tutorial002.py` & `fastapi-0.99.1/docs_src/background_tasks/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/background_tasks/tutorial002_an.py` & `fastapi-0.99.1/docs_src/background_tasks/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/background_tasks/tutorial002_an_py310.py` & `fastapi-0.99.1/docs_src/background_tasks/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/background_tasks/tutorial002_an_py39.py` & `fastapi-0.99.1/docs_src/background_tasks/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/background_tasks/tutorial002_py310.py` & `fastapi-0.99.1/docs_src/background_tasks/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/bigger_applications/app/main.py` & `fastapi-0.99.1/docs_src/bigger_applications/app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/bigger_applications/app/routers/items.py` & `fastapi-0.99.1/docs_src/bigger_applications/app/routers/items.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/bigger_applications/app_an/main.py` & `fastapi-0.99.1/docs_src/bigger_applications/app_an/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/bigger_applications/app_an/routers/items.py` & `fastapi-0.99.1/docs_src/bigger_applications/app_an/routers/items.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/bigger_applications/app_an_py39/main.py` & `fastapi-0.99.1/docs_src/bigger_applications/app_an_py39/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/bigger_applications/app_an_py39/routers/items.py` & `fastapi-0.99.1/docs_src/bigger_applications/app_an_py39/routers/items.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_fields/tutorial001.py` & `fastapi-0.99.1/docs_src/body_fields/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_fields/tutorial001_an.py` & `fastapi-0.99.1/docs_src/body_fields/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_fields/tutorial001_an_py310.py` & `fastapi-0.99.1/docs_src/body_fields/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_fields/tutorial001_an_py39.py` & `fastapi-0.99.1/docs_src/body_fields/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_fields/tutorial001_py310.py` & `fastapi-0.99.1/docs_src/body_fields/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_multiple_params/tutorial001.py` & `fastapi-0.99.1/docs_src/body_multiple_params/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_multiple_params/tutorial001_an.py` & `fastapi-0.99.1/docs_src/body_multiple_params/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_multiple_params/tutorial001_an_py310.py` & `fastapi-0.99.1/docs_src/body_multiple_params/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_multiple_params/tutorial001_an_py39.py` & `fastapi-0.99.1/docs_src/body_multiple_params/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_multiple_params/tutorial001_py310.py` & `fastapi-0.99.1/docs_src/body_multiple_params/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_multiple_params/tutorial003.py` & `fastapi-0.99.1/docs_src/body_multiple_params/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_multiple_params/tutorial003_an.py` & `fastapi-0.99.1/docs_src/body_multiple_params/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_multiple_params/tutorial003_an_py310.py` & `fastapi-0.99.1/docs_src/body_multiple_params/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_multiple_params/tutorial003_an_py39.py` & `fastapi-0.99.1/docs_src/body_multiple_params/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_multiple_params/tutorial004.py` & `fastapi-0.99.1/docs_src/body_multiple_params/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_multiple_params/tutorial004_an.py` & `fastapi-0.99.1/docs_src/body_multiple_params/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_multiple_params/tutorial004_an_py310.py` & `fastapi-0.99.1/docs_src/body_multiple_params/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_multiple_params/tutorial004_an_py39.py` & `fastapi-0.99.1/docs_src/body_multiple_params/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_multiple_params/tutorial004_py310.py` & `fastapi-0.99.1/docs_src/body_multiple_params/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_nested_models/tutorial005.py` & `fastapi-0.99.1/docs_src/body_nested_models/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_nested_models/tutorial005_py39.py` & `fastapi-0.99.1/docs_src/body_nested_models/tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_nested_models/tutorial006.py` & `fastapi-0.99.1/docs_src/body_nested_models/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_nested_models/tutorial006_py39.py` & `fastapi-0.99.1/docs_src/body_nested_models/tutorial006_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_nested_models/tutorial007.py` & `fastapi-0.99.1/docs_src/body_nested_models/tutorial007.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_nested_models/tutorial007_py310.py` & `fastapi-0.99.1/docs_src/body_nested_models/tutorial007_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_nested_models/tutorial007_py39.py` & `fastapi-0.99.1/docs_src/body_nested_models/tutorial007_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_updates/tutorial001.py` & `fastapi-0.99.1/docs_src/body_updates/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_updates/tutorial001_py310.py` & `fastapi-0.99.1/docs_src/body_updates/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_updates/tutorial001_py39.py` & `fastapi-0.99.1/docs_src/body_updates/tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_updates/tutorial002.py` & `fastapi-0.99.1/docs_src/body_updates/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_updates/tutorial002_py310.py` & `fastapi-0.99.1/docs_src/body_updates/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/body_updates/tutorial002_py39.py` & `fastapi-0.99.1/docs_src/body_updates/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/custom_request_and_route/tutorial001.py` & `fastapi-0.99.1/docs_src/custom_request_and_route/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/custom_request_and_route/tutorial002.py` & `fastapi-0.99.1/docs_src/custom_request_and_route/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/custom_request_and_route/tutorial003.py` & `fastapi-0.99.1/docs_src/custom_request_and_route/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dataclasses/tutorial002.py` & `fastapi-0.99.1/docs_src/dataclasses/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dataclasses/tutorial003.py` & `fastapi-0.99.1/docs_src/dataclasses/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial002.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial002_an.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial002_an_py310.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial002_an_py39.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial002_py310.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial003.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial003_an.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial003_an_py310.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial003_an_py39.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial003_py310.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial004.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial004_an.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial004_an_py310.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial004_an_py39.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial004_py310.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial005_an.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial005_an_py39.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial006.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial006_an.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial006_an_py39.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial006_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial008_an.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial008_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial008_an_py39.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial008_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial011_an.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial011_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial011_an_py39.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial011_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial012.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial012.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial012_an.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial012_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependencies/tutorial012_an_py39.py` & `fastapi-0.99.1/docs_src/dependencies/tutorial012_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependency_testing/tutorial001.py` & `fastapi-0.99.1/docs_src/dependency_testing/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependency_testing/tutorial001_an.py` & `fastapi-0.99.1/docs_src/dependency_testing/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependency_testing/tutorial001_an_py310.py` & `fastapi-0.99.1/docs_src/dependency_testing/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependency_testing/tutorial001_an_py39.py` & `fastapi-0.99.1/docs_src/dependency_testing/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/dependency_testing/tutorial001_py310.py` & `fastapi-0.99.1/docs_src/dependency_testing/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/events/tutorial003.py` & `fastapi-0.99.1/docs_src/events/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/extending_openapi/tutorial001.py` & `fastapi-0.99.1/docs_src/extending_openapi/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/extending_openapi/tutorial002.py` & `fastapi-0.99.1/docs_src/extending_openapi/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/extra_data_types/tutorial001.py` & `fastapi-0.99.1/docs_src/extra_data_types/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/extra_data_types/tutorial001_an.py` & `fastapi-0.99.1/docs_src/extra_data_types/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/extra_data_types/tutorial001_an_py310.py` & `fastapi-0.99.1/docs_src/extra_data_types/tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/extra_data_types/tutorial001_an_py39.py` & `fastapi-0.99.1/docs_src/extra_data_types/tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/extra_data_types/tutorial001_py310.py` & `fastapi-0.99.1/docs_src/extra_data_types/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/extra_models/tutorial001.py` & `fastapi-0.99.1/docs_src/extra_models/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/extra_models/tutorial001_py310.py` & `fastapi-0.99.1/docs_src/extra_models/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/extra_models/tutorial002.py` & `fastapi-0.99.1/docs_src/extra_models/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/extra_models/tutorial002_py310.py` & `fastapi-0.99.1/docs_src/extra_models/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/extra_models/tutorial003.py` & `fastapi-0.99.1/docs_src/extra_models/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/extra_models/tutorial003_py310.py` & `fastapi-0.99.1/docs_src/extra_models/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/generate_clients/tutorial001.py` & `fastapi-0.99.1/docs_src/generate_clients/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/generate_clients/tutorial002.py` & `fastapi-0.99.1/docs_src/generate_clients/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/generate_clients/tutorial002_py39.py` & `fastapi-0.99.1/docs_src/generate_clients/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/generate_clients/tutorial003.py` & `fastapi-0.99.1/docs_src/generate_clients/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/generate_clients/tutorial003_py39.py` & `fastapi-0.99.1/docs_src/generate_clients/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/handling_errors/tutorial003.py` & `fastapi-0.99.1/docs_src/handling_errors/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/handling_errors/tutorial004.py` & `fastapi-0.99.1/docs_src/handling_errors/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/handling_errors/tutorial005.py` & `fastapi-0.99.1/docs_src/handling_errors/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/handling_errors/tutorial006.py` & `fastapi-0.99.1/docs_src/handling_errors/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/metadata/tutorial001.py` & `fastapi-0.99.1/docs_src/metadata/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/metadata/tutorial001_1.py` & `fastapi-0.99.1/docs_src/metadata/tutorial001_1.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/metadata/tutorial004.py` & `fastapi-0.99.1/docs_src/metadata/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/nosql_databases/tutorial001.py` & `fastapi-0.99.1/docs_src/nosql_databases/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/openapi_callbacks/tutorial001.py` & `fastapi-0.99.1/docs_src/openapi_callbacks/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/openapi_webhooks/tutorial001.py` & `fastapi-0.99.1/docs_src/openapi_webhooks/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/path_operation_advanced_configuration/tutorial002.py` & `fastapi-0.99.1/docs_src/path_operation_advanced_configuration/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/path_operation_advanced_configuration/tutorial004.py` & `fastapi-0.99.1/docs_src/path_operation_advanced_configuration/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/path_operation_advanced_configuration/tutorial006.py` & `fastapi-0.99.1/docs_src/path_operation_advanced_configuration/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/path_operation_advanced_configuration/tutorial007.py` & `fastapi-0.99.1/docs_src/path_operation_advanced_configuration/tutorial007.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/path_operation_configuration/tutorial002.py` & `fastapi-0.99.1/docs_src/path_operation_configuration/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/path_operation_configuration/tutorial002_py310.py` & `fastapi-0.99.1/docs_src/path_operation_configuration/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/path_operation_configuration/tutorial002_py39.py` & `fastapi-0.99.1/docs_src/path_operation_configuration/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/path_operation_configuration/tutorial003.py` & `fastapi-0.99.1/docs_src/path_operation_configuration/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/path_operation_configuration/tutorial003_py39.py` & `fastapi-0.99.1/docs_src/path_operation_configuration/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/path_operation_configuration/tutorial004.py` & `fastapi-0.99.1/docs_src/path_operation_configuration/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/path_operation_configuration/tutorial004_py310.py` & `fastapi-0.99.1/docs_src/path_operation_configuration/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/path_operation_configuration/tutorial004_py39.py` & `fastapi-0.99.1/docs_src/path_operation_configuration/tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/path_operation_configuration/tutorial005.py` & `fastapi-0.99.1/docs_src/path_operation_configuration/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/path_operation_configuration/tutorial005_py310.py` & `fastapi-0.99.1/docs_src/path_operation_configuration/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/path_operation_configuration/tutorial005_py39.py` & `fastapi-0.99.1/docs_src/path_operation_configuration/tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/path_params/tutorial005.py` & `fastapi-0.99.1/docs_src/path_params/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/query_params_str_validations/tutorial008_an.py` & `fastapi-0.99.1/docs_src/query_params_str_validations/tutorial008_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/query_params_str_validations/tutorial010.py` & `fastapi-0.99.1/docs_src/query_params_str_validations/tutorial010.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/query_params_str_validations/tutorial010_an.py` & `fastapi-0.99.1/docs_src/query_params_str_validations/tutorial010_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/query_params_str_validations/tutorial010_an_py310.py` & `fastapi-0.99.1/docs_src/query_params_str_validations/tutorial010_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/query_params_str_validations/tutorial010_an_py39.py` & `fastapi-0.99.1/docs_src/query_params_str_validations/tutorial010_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/query_params_str_validations/tutorial010_py310.py` & `fastapi-0.99.1/docs_src/query_params_str_validations/tutorial010_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/request_files/tutorial001_02_an.py` & `fastapi-0.99.1/docs_src/request_files/tutorial001_02_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/request_files/tutorial001_02_an_py39.py` & `fastapi-0.99.1/docs_src/request_files/tutorial001_02_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/request_files/tutorial002.py` & `fastapi-0.99.1/docs_src/request_files/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/request_files/tutorial002_an.py` & `fastapi-0.99.1/docs_src/request_files/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/request_files/tutorial002_an_py39.py` & `fastapi-0.99.1/docs_src/request_files/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/request_files/tutorial002_py39.py` & `fastapi-0.99.1/docs_src/request_files/tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/request_files/tutorial003.py` & `fastapi-0.99.1/docs_src/request_files/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/request_files/tutorial003_an.py` & `fastapi-0.99.1/docs_src/request_files/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/request_files/tutorial003_an_py39.py` & `fastapi-0.99.1/docs_src/request_files/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/request_files/tutorial003_py39.py` & `fastapi-0.99.1/docs_src/request_files/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/response_model/tutorial001.py` & `fastapi-0.99.1/docs_src/response_model/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/response_model/tutorial001_01.py` & `fastapi-0.99.1/docs_src/response_model/tutorial001_01.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/response_model/tutorial001_py310.py` & `fastapi-0.99.1/docs_src/response_model/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/response_model/tutorial001_py39.py` & `fastapi-0.99.1/docs_src/response_model/tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/response_model/tutorial004.py` & `fastapi-0.99.1/docs_src/response_model/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/response_model/tutorial004_py310.py` & `fastapi-0.99.1/docs_src/response_model/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/response_model/tutorial004_py39.py` & `fastapi-0.99.1/docs_src/response_model/tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/response_model/tutorial005.py` & `fastapi-0.99.1/docs_src/response_model/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/response_model/tutorial005_py310.py` & `fastapi-0.99.1/docs_src/response_model/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/response_model/tutorial006.py` & `fastapi-0.99.1/docs_src/response_model/tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/response_model/tutorial006_py310.py` & `fastapi-0.99.1/docs_src/response_model/tutorial006_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/schema_extra_example/tutorial001.py` & `fastapi-0.99.1/docs_src/schema_extra_example/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/schema_extra_example/tutorial001_py310.py` & `fastapi-0.99.1/docs_src/schema_extra_example/tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/schema_extra_example/tutorial002.py` & `fastapi-0.99.1/docs_src/schema_extra_example/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/schema_extra_example/tutorial003.py` & `fastapi-0.99.1/docs_src/schema_extra_example/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/schema_extra_example/tutorial003_an.py` & `fastapi-0.99.1/docs_src/schema_extra_example/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/schema_extra_example/tutorial003_an_py310.py` & `fastapi-0.99.1/docs_src/schema_extra_example/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/schema_extra_example/tutorial003_an_py39.py` & `fastapi-0.99.1/docs_src/schema_extra_example/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/schema_extra_example/tutorial003_py310.py` & `fastapi-0.99.1/docs_src/schema_extra_example/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/schema_extra_example/tutorial004_py310.py` & `fastapi-0.99.1/docs_src/schema_extra_example/tutorial004_an.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,44 @@
+from typing import Union
+
 from fastapi import Body, FastAPI
 from pydantic import BaseModel
+from typing_extensions import Annotated
 
 app = FastAPI()
 
 
 class Item(BaseModel):
     name: str
-    description: str | None = None
+    description: Union[str, None] = None
     price: float
-    tax: float | None = None
+    tax: Union[float, None] = None
 
 
 @app.put("/items/{item_id}")
 async def update_item(
     *,
     item_id: int,
-    item: Item = Body(
-        examples=[
-            {
-                "summary": "A normal example",
-                "description": "A **normal** item works correctly.",
-                "value": {
+    item: Annotated[
+        Item,
+        Body(
+            examples=[
+                {
                     "name": "Foo",
                     "description": "A very nice Item",
                     "price": 35.4,
                     "tax": 3.2,
                 },
-            },
-            {
-                "summary": "An example with converted data",
-                "description": "FastAPI can convert price `strings` to actual `numbers` automatically",
-                "value": {
+                {
                     "name": "Bar",
                     "price": "35.4",
                 },
-            },
-            {
-                "summary": "Invalid data is rejected with an error",
-                "value": {
+                {
                     "name": "Baz",
                     "price": "thirty five point four",
                 },
-            },
-        ],
-    ),
+            ],
+        ),
+    ],
 ):
     results = {"item_id": item_id, "item": item}
     return results
```

### Comparing `fastapi-0.99.0/docs_src/security/tutorial002.py` & `fastapi-0.99.1/docs_src/security/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial002_an.py` & `fastapi-0.99.1/docs_src/security/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial002_an_py310.py` & `fastapi-0.99.1/docs_src/security/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial002_an_py39.py` & `fastapi-0.99.1/docs_src/security/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial002_py310.py` & `fastapi-0.99.1/docs_src/security/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial003.py` & `fastapi-0.99.1/docs_src/security/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial003_an.py` & `fastapi-0.99.1/docs_src/security/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial003_an_py310.py` & `fastapi-0.99.1/docs_src/security/tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial003_an_py39.py` & `fastapi-0.99.1/docs_src/security/tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial003_py310.py` & `fastapi-0.99.1/docs_src/security/tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial004.py` & `fastapi-0.99.1/docs_src/security/tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial004_an.py` & `fastapi-0.99.1/docs_src/security/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial004_an_py310.py` & `fastapi-0.99.1/docs_src/security/tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial004_an_py39.py` & `fastapi-0.99.1/docs_src/security/tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial004_py310.py` & `fastapi-0.99.1/docs_src/security/tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial005.py` & `fastapi-0.99.1/docs_src/security/tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial005_an.py` & `fastapi-0.99.1/docs_src/security/tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial005_an_py310.py` & `fastapi-0.99.1/docs_src/security/tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial005_an_py39.py` & `fastapi-0.99.1/docs_src/security/tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial005_py310.py` & `fastapi-0.99.1/docs_src/security/tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial005_py39.py` & `fastapi-0.99.1/docs_src/security/tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial007.py` & `fastapi-0.99.1/docs_src/security/tutorial007.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial007_an.py` & `fastapi-0.99.1/docs_src/security/tutorial007_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/security/tutorial007_an_py39.py` & `fastapi-0.99.1/docs_src/security/tutorial007_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/settings/app02/test_main.py` & `fastapi-0.99.1/docs_src/settings/app02/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/settings/app02_an/test_main.py` & `fastapi-0.99.1/docs_src/settings/app02_an/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/settings/app02_an_py39/test_main.py` & `fastapi-0.99.1/docs_src/settings/app02_an_py39/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/sql_databases/sql_app/alt_main.py` & `fastapi-0.99.1/docs_src/sql_databases/sql_app/alt_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/sql_databases/sql_app/crud.py` & `fastapi-0.99.1/docs_src/sql_databases/sql_app/crud.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/sql_databases/sql_app/main.py` & `fastapi-0.99.1/docs_src/sql_databases/sql_app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/sql_databases/sql_app/models.py` & `fastapi-0.99.1/docs_src/sql_databases/sql_app/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/sql_databases/sql_app/tests/test_sql_app.py` & `fastapi-0.99.1/docs_src/sql_databases/sql_app/tests/test_sql_app.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/sql_databases/sql_app_py310/alt_main.py` & `fastapi-0.99.1/docs_src/sql_databases/sql_app_py310/alt_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/sql_databases/sql_app_py310/crud.py` & `fastapi-0.99.1/docs_src/sql_databases/sql_app_py310/crud.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/sql_databases/sql_app_py310/main.py` & `fastapi-0.99.1/docs_src/sql_databases/sql_app_py310/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/sql_databases/sql_app_py310/models.py` & `fastapi-0.99.1/docs_src/sql_databases/sql_app_py310/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py` & `fastapi-0.99.1/docs_src/sql_databases/sql_app_py310/tests/test_sql_app.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/sql_databases/sql_app_py39/alt_main.py` & `fastapi-0.99.1/docs_src/sql_databases/sql_app_py39/alt_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/sql_databases/sql_app_py39/crud.py` & `fastapi-0.99.1/docs_src/sql_databases/sql_app_py39/crud.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/sql_databases/sql_app_py39/main.py` & `fastapi-0.99.1/docs_src/sql_databases/sql_app_py39/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/sql_databases/sql_app_py39/models.py` & `fastapi-0.99.1/docs_src/sql_databases/sql_app_py39/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py` & `fastapi-0.99.1/docs_src/sql_databases/sql_app_py39/tests/test_sql_app.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/sql_databases_peewee/sql_app/crud.py` & `fastapi-0.99.1/docs_src/sql_databases_peewee/sql_app/crud.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/sql_databases_peewee/sql_app/database.py` & `fastapi-0.99.1/docs_src/sql_databases_peewee/sql_app/database.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/sql_databases_peewee/sql_app/main.py` & `fastapi-0.99.1/docs_src/sql_databases_peewee/sql_app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/sql_databases_peewee/sql_app/schemas.py` & `fastapi-0.99.1/docs_src/sql_databases_peewee/sql_app/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/websockets/tutorial001.py` & `fastapi-0.99.1/docs_src/websockets/tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/websockets/tutorial002.py` & `fastapi-0.99.1/docs_src/websockets/tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/websockets/tutorial002_an.py` & `fastapi-0.99.1/docs_src/websockets/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/websockets/tutorial002_an_py310.py` & `fastapi-0.99.1/docs_src/websockets/tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/websockets/tutorial002_an_py39.py` & `fastapi-0.99.1/docs_src/websockets/tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/websockets/tutorial002_py310.py` & `fastapi-0.99.1/docs_src/websockets/tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/websockets/tutorial003.py` & `fastapi-0.99.1/docs_src/websockets/tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/docs_src/websockets/tutorial003_py39.py` & `fastapi-0.99.1/docs_src/websockets/tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/__init__.py` & `fastapi-0.99.1/fastapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """FastAPI framework, high performance, easy to learn, fast to code, ready for production"""
 
-__version__ = "0.99.0"
+__version__ = "0.99.1"
 
 from starlette import status as status
 
 from .applications import FastAPI as FastAPI
 from .background import BackgroundTasks as BackgroundTasks
 from .datastructures import UploadFile as UploadFile
 from .exceptions import HTTPException as HTTPException
```

### Comparing `fastapi-0.99.0/fastapi/applications.py` & `fastapi-0.99.1/fastapi/applications.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/concurrency.py` & `fastapi-0.99.1/fastapi/concurrency.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/datastructures.py` & `fastapi-0.99.1/fastapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/encoders.py` & `fastapi-0.99.1/fastapi/encoders.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/exception_handlers.py` & `fastapi-0.99.1/fastapi/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/exceptions.py` & `fastapi-0.99.1/fastapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/param_functions.py` & `fastapi-0.99.1/fastapi/param_functions.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/params.py` & `fastapi-0.99.1/fastapi/params.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/responses.py` & `fastapi-0.99.1/fastapi/responses.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/routing.py` & `fastapi-0.99.1/fastapi/routing.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/utils.py` & `fastapi-0.99.1/fastapi/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/dependencies/models.py` & `fastapi-0.99.1/fastapi/dependencies/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/dependencies/utils.py` & `fastapi-0.99.1/fastapi/dependencies/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/middleware/asyncexitstack.py` & `fastapi-0.99.1/fastapi/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/openapi/docs.py` & `fastapi-0.99.1/fastapi/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/openapi/models.py` & `fastapi-0.99.1/fastapi/openapi/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -110,35 +110,38 @@
     schema_: Optional[str] = Field(default=None, alias="$schema")
     vocabulary: Optional[str] = Field(default=None, alias="$vocabulary")
     id: Optional[str] = Field(default=None, alias="$id")
     anchor: Optional[str] = Field(default=None, alias="$anchor")
     dynamicAnchor: Optional[str] = Field(default=None, alias="$dynamicAnchor")
     ref: Optional[str] = Field(default=None, alias="$ref")
     dynamicRef: Optional[str] = Field(default=None, alias="$dynamicRef")
-    defs: Optional[Dict[str, "Schema"]] = Field(default=None, alias="$defs")
+    defs: Optional[Dict[str, "SchemaOrBool"]] = Field(default=None, alias="$defs")
     comment: Optional[str] = Field(default=None, alias="$comment")
     # Ref: JSON Schema 2020-12: https://json-schema.org/draft/2020-12/json-schema-core.html#name-a-vocabulary-for-applying-s
     # A Vocabulary for Applying Subschemas
-    allOf: Optional[List["Schema"]] = None
-    anyOf: Optional[List["Schema"]] = None
-    oneOf: Optional[List["Schema"]] = None
-    not_: Optional["Schema"] = Field(default=None, alias="not")
-    if_: Optional["Schema"] = Field(default=None, alias="if")
-    then: Optional["Schema"] = None
-    else_: Optional["Schema"] = Field(default=None, alias="else")
-    dependentSchemas: Optional[Dict[str, "Schema"]] = None
-    prefixItems: Optional[List["Schema"]] = None
-    items: Optional[Union["Schema", List["Schema"]]] = None
-    contains: Optional["Schema"] = None
-    properties: Optional[Dict[str, "Schema"]] = None
-    patternProperties: Optional[Dict[str, "Schema"]] = None
-    additionalProperties: Optional["Schema"] = None
-    propertyNames: Optional["Schema"] = None
-    unevaluatedItems: Optional["Schema"] = None
-    unevaluatedProperties: Optional["Schema"] = None
+    allOf: Optional[List["SchemaOrBool"]] = None
+    anyOf: Optional[List["SchemaOrBool"]] = None
+    oneOf: Optional[List["SchemaOrBool"]] = None
+    not_: Optional["SchemaOrBool"] = Field(default=None, alias="not")
+    if_: Optional["SchemaOrBool"] = Field(default=None, alias="if")
+    then: Optional["SchemaOrBool"] = None
+    else_: Optional["SchemaOrBool"] = Field(default=None, alias="else")
+    dependentSchemas: Optional[Dict[str, "SchemaOrBool"]] = None
+    prefixItems: Optional[List["SchemaOrBool"]] = None
+    # TODO: uncomment and remove below when deprecating Pydantic v1
+    # It generales a list of schemas for tuples, before prefixItems was available
+    # items: Optional["SchemaOrBool"] = None
+    items: Optional[Union["SchemaOrBool", List["SchemaOrBool"]]] = None
+    contains: Optional["SchemaOrBool"] = None
+    properties: Optional[Dict[str, "SchemaOrBool"]] = None
+    patternProperties: Optional[Dict[str, "SchemaOrBool"]] = None
+    additionalProperties: Optional["SchemaOrBool"] = None
+    propertyNames: Optional["SchemaOrBool"] = None
+    unevaluatedItems: Optional["SchemaOrBool"] = None
+    unevaluatedProperties: Optional["SchemaOrBool"] = None
     # Ref: JSON Schema Validation 2020-12: https://json-schema.org/draft/2020-12/json-schema-validation.html#name-a-vocabulary-for-structural
     # A Vocabulary for Structural Validation
     type: Optional[str] = None
     enum: Optional[List[Any]] = None
     const: Optional[Any] = None
     multipleOf: Optional[float] = Field(default=None, gt=0)
     maximum: Optional[float] = None
@@ -160,15 +163,15 @@
     # Ref: JSON Schema Validation 2020-12: https://json-schema.org/draft/2020-12/json-schema-validation.html#name-vocabularies-for-semantic-c
     # Vocabularies for Semantic Content With "format"
     format: Optional[str] = None
     # Ref: JSON Schema Validation 2020-12: https://json-schema.org/draft/2020-12/json-schema-validation.html#name-a-vocabulary-for-the-conten
     # A Vocabulary for the Contents of String-Encoded Data
     contentEncoding: Optional[str] = None
     contentMediaType: Optional[str] = None
-    contentSchema: Optional["Schema"] = None
+    contentSchema: Optional["SchemaOrBool"] = None
     # Ref: JSON Schema Validation 2020-12: https://json-schema.org/draft/2020-12/json-schema-validation.html#name-a-vocabulary-for-basic-meta
     # A Vocabulary for Basic Meta-Data Annotations
     title: Optional[str] = None
     description: Optional[str] = None
     default: Optional[Any] = None
     deprecated: Optional[bool] = None
     readOnly: Optional[bool] = None
@@ -187,14 +190,19 @@
         ),
     ] = None
 
     class Config:
         extra: str = "allow"
 
 
+# Ref: https://json-schema.org/draft/2020-12/json-schema-core.html#name-json-schema-documents
+# A JSON Schema MUST be an object or a boolean.
+SchemaOrBool = Union[Schema, bool]
+
+
 class Example(BaseModel):
     summary: Optional[str] = None
     description: Optional[str] = None
     value: Optional[Any] = None
     externalValue: Optional[AnyUrl] = None
 
     class Config:
```

### Comparing `fastapi-0.99.0/fastapi/openapi/utils.py` & `fastapi-0.99.1/fastapi/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/security/__init__.py` & `fastapi-0.99.1/fastapi/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/security/api_key.py` & `fastapi-0.99.1/fastapi/security/api_key.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/security/http.py` & `fastapi-0.99.1/fastapi/security/http.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/security/oauth2.py` & `fastapi-0.99.1/fastapi/security/oauth2.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/fastapi/security/open_id_connect_url.py` & `fastapi-0.99.1/fastapi/security/open_id_connect_url.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/scripts/docs.py` & `fastapi-0.99.1/scripts/docs.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/scripts/gitter_releases_bot.py` & `fastapi-0.99.1/scripts/gitter_releases_bot.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/scripts/mkdocs_hooks.py` & `fastapi-0.99.1/scripts/mkdocs_hooks.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/main.py` & `fastapi-0.99.1/tests/main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_additional_properties.py` & `fastapi-0.99.1/tests/test_additional_properties.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_additional_response_extra.py` & `fastapi-0.99.1/tests/test_additional_response_extra.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_additional_responses_bad.py` & `fastapi-0.99.1/tests/test_additional_responses_bad.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_additional_responses_custom_model_in_callback.py` & `fastapi-0.99.1/tests/test_additional_responses_custom_model_in_callback.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_additional_responses_custom_validationerror.py` & `fastapi-0.99.1/tests/test_additional_responses_custom_validationerror.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_additional_responses_default_validationerror.py` & `fastapi-0.99.1/tests/test_additional_responses_default_validationerror.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_additional_responses_response_class.py` & `fastapi-0.99.1/tests/test_additional_responses_response_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_additional_responses_router.py` & `fastapi-0.99.1/tests/test_additional_responses_router.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_ambiguous_params.py` & `fastapi-0.99.1/tests/test_ambiguous_params.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_annotated.py` & `fastapi-0.99.1/tests/test_annotated.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_application.py` & `fastapi-0.99.1/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_custom_middleware_exception.py` & `fastapi-0.99.1/tests/test_custom_middleware_exception.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_custom_route_class.py` & `fastapi-0.99.1/tests/test_custom_route_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_custom_schema_fields.py` & `fastapi-0.99.1/tests/test_custom_schema_fields.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_custom_swagger_ui_redirect.py` & `fastapi-0.99.1/tests/test_custom_swagger_ui_redirect.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_datastructures.py` & `fastapi-0.99.1/tests/test_datastructures.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_datetime_custom_encoder.py` & `fastapi-0.99.1/tests/test_datetime_custom_encoder.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_default_response_class.py` & `fastapi-0.99.1/tests/test_default_response_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_default_response_class_router.py` & `fastapi-0.99.1/tests/test_default_response_class_router.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_dependency_cache.py` & `fastapi-0.99.1/tests/test_dependency_cache.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_dependency_class.py` & `fastapi-0.99.1/tests/test_dependency_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_dependency_contextmanager.py` & `fastapi-0.99.1/tests/test_dependency_contextmanager.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_dependency_contextvars.py` & `fastapi-0.99.1/tests/test_dependency_contextvars.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_dependency_duplicates.py` & `fastapi-0.99.1/tests/test_dependency_duplicates.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_dependency_normal_exceptions.py` & `fastapi-0.99.1/tests/test_dependency_normal_exceptions.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_dependency_overrides.py` & `fastapi-0.99.1/tests/test_dependency_overrides.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_dependency_security_overrides.py` & `fastapi-0.99.1/tests/test_dependency_security_overrides.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_deprecated_openapi_prefix.py` & `fastapi-0.99.1/tests/test_deprecated_openapi_prefix.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_duplicate_models_openapi.py` & `fastapi-0.99.1/tests/test_duplicate_models_openapi.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_empty_router.py` & `fastapi-0.99.1/tests/test_empty_router.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_enforce_once_required_parameter.py` & `fastapi-0.99.1/tests/test_enforce_once_required_parameter.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_exception_handlers.py` & `fastapi-0.99.1/tests/test_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_extra_routes.py` & `fastapi-0.99.1/tests/test_extra_routes.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_filter_pydantic_sub_model.py` & `fastapi-0.99.1/tests/test_filter_pydantic_sub_model.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_forms_from_non_typing_sequences.py` & `fastapi-0.99.1/tests/test_forms_from_non_typing_sequences.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_generate_unique_id_function.py` & `fastapi-0.99.1/tests/test_generate_unique_id_function.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_get_request_body.py` & `fastapi-0.99.1/tests/test_get_request_body.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_http_connection_injection.py` & `fastapi-0.99.1/tests/test_http_connection_injection.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_include_router_defaults_overrides.py` & `fastapi-0.99.1/tests/test_include_router_defaults_overrides.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_infer_param_optionality.py` & `fastapi-0.99.1/tests/test_infer_param_optionality.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_inherited_custom_class.py` & `fastapi-0.99.1/tests/test_inherited_custom_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_invalid_path_param.py` & `fastapi-0.99.1/tests/test_invalid_path_param.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_invalid_sequence_param.py` & `fastapi-0.99.1/tests/test_invalid_sequence_param.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_jsonable_encoder.py` & `fastapi-0.99.1/tests/test_jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_local_docs.py` & `fastapi-0.99.1/tests/test_local_docs.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_multi_body_errors.py` & `fastapi-0.99.1/tests/test_multi_body_errors.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_multi_query_errors.py` & `fastapi-0.99.1/tests/test_multi_query_errors.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_multipart_installation.py` & `fastapi-0.99.1/tests/test_multipart_installation.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_no_swagger_ui_redirect.py` & `fastapi-0.99.1/tests/test_no_swagger_ui_redirect.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_openapi_query_parameter_extension.py` & `fastapi-0.99.1/tests/test_openapi_query_parameter_extension.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_openapi_route_extensions.py` & `fastapi-0.99.1/tests/test_openapi_route_extensions.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_openapi_servers.py` & `fastapi-0.99.1/tests/test_openapi_servers.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_operations_signatures.py` & `fastapi-0.99.1/tests/test_operations_signatures.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_orjson_response_class.py` & `fastapi-0.99.1/tests/test_orjson_response_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_param_class.py` & `fastapi-0.99.1/tests/test_param_class.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_param_in_path_and_dependency.py` & `fastapi-0.99.1/tests/test_param_in_path_and_dependency.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_param_include_in_schema.py` & `fastapi-0.99.1/tests/test_param_include_in_schema.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_params_repr.py` & `fastapi-0.99.1/tests/test_params_repr.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_path.py` & `fastapi-0.99.1/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_put_no_body.py` & `fastapi-0.99.1/tests/test_put_no_body.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_query.py` & `fastapi-0.99.1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_read_with_orm_mode.py` & `fastapi-0.99.1/tests/test_read_with_orm_mode.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_repeated_cookie_headers.py` & `fastapi-0.99.1/tests/test_repeated_cookie_headers.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_repeated_dependency_schema.py` & `fastapi-0.99.1/tests/test_repeated_dependency_schema.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_repeated_parameter_alias.py` & `fastapi-0.99.1/tests/test_repeated_parameter_alias.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_reponse_set_reponse_code_empty.py` & `fastapi-0.99.1/tests/test_reponse_set_reponse_code_empty.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_request_body_parameters_media_type.py` & `fastapi-0.99.1/tests/test_request_body_parameters_media_type.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_required_noneable.py` & `fastapi-0.99.1/tests/test_required_noneable.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_response_by_alias.py` & `fastapi-0.99.1/tests/test_response_by_alias.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_response_change_status_code.py` & `fastapi-0.99.1/tests/test_response_change_status_code.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_response_class_no_mediatype.py` & `fastapi-0.99.1/tests/test_response_class_no_mediatype.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_response_code_no_body.py` & `fastapi-0.99.1/tests/test_response_code_no_body.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_response_model_as_return_annotation.py` & `fastapi-0.99.1/tests/test_response_model_as_return_annotation.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_response_model_include_exclude.py` & `fastapi-0.99.1/tests/test_response_model_include_exclude.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_response_model_invalid.py` & `fastapi-0.99.1/tests/test_response_model_invalid.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_response_model_sub_types.py` & `fastapi-0.99.1/tests/test_response_model_sub_types.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_route_scope.py` & `fastapi-0.99.1/tests/test_route_scope.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_router_events.py` & `fastapi-0.99.1/tests/test_router_events.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_router_redirect_slashes.py` & `fastapi-0.99.1/tests/test_router_redirect_slashes.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_schema_extra_examples.py` & `fastapi-0.99.1/tests/test_schema_extra_examples.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_api_key_cookie.py` & `fastapi-0.99.1/tests/test_security_api_key_cookie.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_api_key_cookie_description.py` & `fastapi-0.99.1/tests/test_security_api_key_cookie_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_api_key_cookie_optional.py` & `fastapi-0.99.1/tests/test_security_api_key_cookie_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_api_key_header.py` & `fastapi-0.99.1/tests/test_security_api_key_header.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_api_key_header_description.py` & `fastapi-0.99.1/tests/test_security_api_key_header_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_api_key_header_optional.py` & `fastapi-0.99.1/tests/test_security_api_key_header_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_api_key_query.py` & `fastapi-0.99.1/tests/test_security_api_key_query.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_api_key_query_description.py` & `fastapi-0.99.1/tests/test_security_api_key_query_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_api_key_query_optional.py` & `fastapi-0.99.1/tests/test_security_api_key_query_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_http_base.py` & `fastapi-0.99.1/tests/test_security_http_base.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_http_base_description.py` & `fastapi-0.99.1/tests/test_security_http_base_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_http_base_optional.py` & `fastapi-0.99.1/tests/test_security_http_base_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_http_basic_optional.py` & `fastapi-0.99.1/tests/test_security_http_basic_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_http_basic_realm.py` & `fastapi-0.99.1/tests/test_security_http_basic_realm.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_http_basic_realm_description.py` & `fastapi-0.99.1/tests/test_security_http_basic_realm_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_http_bearer.py` & `fastapi-0.99.1/tests/test_security_http_bearer.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_http_bearer_description.py` & `fastapi-0.99.1/tests/test_security_http_bearer_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_http_bearer_optional.py` & `fastapi-0.99.1/tests/test_security_http_bearer_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_http_digest.py` & `fastapi-0.99.1/tests/test_security_http_digest.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_http_digest_description.py` & `fastapi-0.99.1/tests/test_security_http_digest_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_http_digest_optional.py` & `fastapi-0.99.1/tests/test_security_http_digest_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_oauth2.py` & `fastapi-0.99.1/tests/test_security_oauth2.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_oauth2_authorization_code_bearer.py` & `fastapi-0.99.1/tests/test_security_oauth2_authorization_code_bearer.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_oauth2_authorization_code_bearer_description.py` & `fastapi-0.99.1/tests/test_security_oauth2_authorization_code_bearer_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_oauth2_optional.py` & `fastapi-0.99.1/tests/test_security_oauth2_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_oauth2_optional_description.py` & `fastapi-0.99.1/tests/test_security_oauth2_optional_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_oauth2_password_bearer_optional.py` & `fastapi-0.99.1/tests/test_security_oauth2_password_bearer_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_oauth2_password_bearer_optional_description.py` & `fastapi-0.99.1/tests/test_security_oauth2_password_bearer_optional_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_openid_connect.py` & `fastapi-0.99.1/tests/test_security_openid_connect.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_openid_connect_description.py` & `fastapi-0.99.1/tests/test_security_openid_connect_description.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_security_openid_connect_optional.py` & `fastapi-0.99.1/tests/test_security_openid_connect_optional.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_serialize_response.py` & `fastapi-0.99.1/tests/test_serialize_response.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_serialize_response_dataclass.py` & `fastapi-0.99.1/tests/test_serialize_response_dataclass.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_serialize_response_model.py` & `fastapi-0.99.1/tests/test_serialize_response_model.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_skip_defaults.py` & `fastapi-0.99.1/tests/test_skip_defaults.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_starlette_exception.py` & `fastapi-0.99.1/tests/test_starlette_exception.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_starlette_urlconvertors.py` & `fastapi-0.99.1/tests/test_starlette_urlconvertors.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_sub_callbacks.py` & `fastapi-0.99.1/tests/test_sub_callbacks.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_swagger_ui_init_oauth.py` & `fastapi-0.99.1/tests/test_swagger_ui_init_oauth.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tuples.py` & `fastapi-0.99.1/tests/test_tuples.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_typing_python39.py` & `fastapi-0.99.1/tests/test_typing_python39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_union_body.py` & `fastapi-0.99.1/tests/test_union_body.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_union_inherited_body.py` & `fastapi-0.99.1/tests/test_union_inherited_body.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_validate_response.py` & `fastapi-0.99.1/tests/test_validate_response.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_validate_response_dataclass.py` & `fastapi-0.99.1/tests/test_validate_response_dataclass.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_validate_response_recursive.py` & `fastapi-0.99.1/tests/test_validate_response_recursive.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_webhooks_security.py` & `fastapi-0.99.1/tests/test_webhooks_security.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_ws_dependencies.py` & `fastapi-0.99.1/tests/test_ws_dependencies.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_ws_router.py` & `fastapi-0.99.1/tests/test_ws_router.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_modules_same_name_body/test_main.py` & `fastapi-0.99.1/tests/test_modules_same_name_body/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_additional_responses/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_additional_responses/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_additional_responses/test_tutorial002.py` & `fastapi-0.99.1/tests/test_tutorial/test_additional_responses/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_additional_responses/test_tutorial003.py` & `fastapi-0.99.1/tests/test_tutorial/test_additional_responses/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_additional_responses/test_tutorial004.py` & `fastapi-0.99.1/tests/test_tutorial/test_additional_responses/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_additional_status_codes/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py` & `fastapi-0.99.1/tests/test_tutorial/test_advanced_middleware/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py` & `fastapi-0.99.1/tests/test_tutorial/test_advanced_middleware/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_async_sql_databases/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_background_tasks/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_background_tasks/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_background_tasks/test_tutorial002.py` & `fastapi-0.99.1/tests/test_tutorial/test_background_tasks/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_background_tasks/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_background_tasks/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_background_tasks/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_behind_a_proxy/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py` & `fastapi-0.99.1/tests/test_tutorial/test_behind_a_proxy/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py` & `fastapi-0.99.1/tests/test_tutorial/test_behind_a_proxy/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py` & `fastapi-0.99.1/tests/test_tutorial/test_behind_a_proxy/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_bigger_applications/test_main.py` & `fastapi-0.99.1/tests/test_tutorial/test_bigger_applications/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_bigger_applications/test_main_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_bigger_applications/test_main_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_bigger_applications/test_main_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_body/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body/test_tutorial001_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_body/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_fields/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_fields/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_fields/test_tutorial001_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_fields/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_fields/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_fields/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_multiple_params/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_nested_models/test_tutorial009.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_nested_models/test_tutorial009.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_nested_models/test_tutorial009_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_updates/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_updates/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_updates/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_body_updates/test_tutorial001_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_conditional_openapi/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_cookie_params/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_cookie_params/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_cookie_params/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_cookie_params/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_cookie_params/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_cors/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_cors/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_custom_request_and_route/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py` & `fastapi-0.99.1/tests/test_tutorial/test_custom_request_and_route/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py` & `fastapi-0.99.1/tests/test_tutorial/test_custom_request_and_route/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_custom_response/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_custom_response/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_custom_response/test_tutorial001b.py` & `fastapi-0.99.1/tests/test_tutorial/test_custom_response/test_tutorial001b.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_custom_response/test_tutorial004.py` & `fastapi-0.99.1/tests/test_tutorial/test_custom_response/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_custom_response/test_tutorial005.py` & `fastapi-0.99.1/tests/test_tutorial/test_custom_response/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_custom_response/test_tutorial006.py` & `fastapi-0.99.1/tests/test_tutorial/test_custom_response/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_custom_response/test_tutorial006b.py` & `fastapi-0.99.1/tests/test_tutorial/test_custom_response/test_tutorial006b.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_custom_response/test_tutorial006c.py` & `fastapi-0.99.1/tests/test_tutorial/test_custom_response/test_tutorial006c.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_dataclasses/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_dataclasses/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_dataclasses/test_tutorial002.py` & `fastapi-0.99.1/tests/test_tutorial/test_dataclasses/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_dataclasses/test_tutorial003.py` & `fastapi-0.99.1/tests/test_tutorial/test_dataclasses/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial001_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial004.py` & `fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial004_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial004_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial006.py` & `fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial006_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial006_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial012.py` & `fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial012.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial012_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial012_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_dependencies/test_tutorial012_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_events/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_events/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_events/test_tutorial002.py` & `fastapi-0.99.1/tests/test_tutorial/test_events/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_events/test_tutorial003.py` & `fastapi-0.99.1/tests/test_tutorial/test_events/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_extending_openapi/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_extending_openapi/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_extending_openapi/test_tutorial002.py` & `fastapi-0.99.1/tests/test_tutorial/test_extending_openapi/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_extending_openapi/test_tutorial003.py` & `fastapi-0.99.1/tests/test_tutorial/test_extending_openapi/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_extending_openapi/test_tutorial004.py` & `fastapi-0.99.1/tests/test_tutorial/test_extending_openapi/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_extending_openapi/test_tutorial005.py` & `fastapi-0.99.1/tests/test_tutorial/test_extending_openapi/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_extra_data_types/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_extra_data_types/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_extra_data_types/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_extra_data_types/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_extra_models/test_tutorial003.py` & `fastapi-0.99.1/tests/test_tutorial/test_extra_models/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_extra_models/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_extra_models/test_tutorial004.py` & `fastapi-0.99.1/tests/test_tutorial/test_extra_models/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_extra_models/test_tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_extra_models/test_tutorial005.py` & `fastapi-0.99.1/tests/test_tutorial/test_extra_models/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_extra_models/test_tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_first_steps/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_first_steps/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_generate_clients/test_tutorial003.py` & `fastapi-0.99.1/tests/test_tutorial/test_generate_clients/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_handling_errors/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_handling_errors/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_handling_errors/test_tutorial002.py` & `fastapi-0.99.1/tests/test_tutorial/test_handling_errors/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_handling_errors/test_tutorial003.py` & `fastapi-0.99.1/tests/test_tutorial/test_handling_errors/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_handling_errors/test_tutorial004.py` & `fastapi-0.99.1/tests/test_tutorial/test_handling_errors/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_handling_errors/test_tutorial005.py` & `fastapi-0.99.1/tests/test_tutorial/test_handling_errors/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_handling_errors/test_tutorial006.py` & `fastapi-0.99.1/tests/test_tutorial/test_handling_errors/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial001_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial001_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial002.py` & `fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial002_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial002_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial003.py` & `fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial003_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_header_params/test_tutorial003_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_header_params/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_metadata/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_metadata/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_metadata/test_tutorial001_1.py` & `fastapi-0.99.1/tests/test_tutorial/test_metadata/test_tutorial001_1.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_metadata/test_tutorial004.py` & `fastapi-0.99.1/tests/test_tutorial/test_metadata/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_openapi_callbacks/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_openapi_webhooks/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_openapi_webhooks/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py` & `fastapi-0.99.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py` & `fastapi-0.99.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py` & `fastapi-0.99.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py` & `fastapi-0.99.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py` & `fastapi-0.99.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py` & `fastapi-0.99.1/tests/test_tutorial/test_path_operation_advanced_configurations/test_tutorial007.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py` & `fastapi-0.99.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial002b.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py` & `fastapi-0.99.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py` & `fastapi-0.99.1/tests/test_tutorial/test_path_operation_configurations/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_path_params/test_tutorial004.py` & `fastapi-0.99.1/tests/test_tutorial/test_path_params/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_path_params/test_tutorial005.py` & `fastapi-0.99.1/tests/test_tutorial/test_path_params/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params/test_tutorial005.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params/test_tutorial006.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params/test_tutorial006_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params/test_tutorial006_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial010_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial011_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial012_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial013_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_query_params_str_validations/test_tutorial014_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_02.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_02.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_02_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_02_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_02_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_03.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_03.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_03_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_03_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial002.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial002_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial002_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial002_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial003.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial003_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_files/test_tutorial003_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_files/test_tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_forms/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_forms/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_forms/test_tutorial001_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_forms/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_forms/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_request_forms_and_files/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_response_change_status_code/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial003.py` & `fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial003_01.py` & `fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial003_01.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial003_01_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial003_02.py` & `fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial003_02.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial003_03.py` & `fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial003_03.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial003_05.py` & `fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial003_05.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial003_05_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial003_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial004.py` & `fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial004_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial004_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial004_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial004_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial005.py` & `fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial005_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial006.py` & `fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_response_model/test_tutorial006_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_response_model/test_tutorial006_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py` & `fastapi-0.99.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,38 @@
+import pytest
 from fastapi.testclient import TestClient
 
-from docs_src.schema_extra_example.tutorial004 import app
+from ...utils import needs_py310
 
-client = TestClient(app)
+
+@pytest.fixture(name="client")
+def get_client():
+    from docs_src.schema_extra_example.tutorial004_py310 import app
+
+    client = TestClient(app)
+    return client
 
 
 # Test required and embedded body parameters with no bodies sent
-def test_post_body_example():
+@needs_py310
+def test_post_body_example(client: TestClient):
     response = client.put(
         "/items/5",
         json={
             "name": "Foo",
             "description": "A very nice Item",
             "price": 35.4,
             "tax": 3.2,
         },
     )
     assert response.status_code == 200
 
 
-def test_openapi_schema():
+@needs_py310
+def test_openapi_schema(client: TestClient):
     response = client.get("/openapi.json")
     assert response.status_code == 200, response.text
     assert response.json() == {
         "openapi": "3.1.0",
         "info": {"title": "FastAPI", "version": "0.1.0"},
         "paths": {
             "/items/{item_id}": {
@@ -42,34 +51,23 @@
                         "content": {
                             "application/json": {
                                 "schema": {
                                     "allOf": [{"$ref": "#/components/schemas/Item"}],
                                     "title": "Item",
                                     "examples": [
                                         {
-                                            "summary": "A normal example",
-                                            "description": "A **normal** item works correctly.",
-                                            "value": {
-                                                "name": "Foo",
-                                                "description": "A very nice Item",
-                                                "price": 35.4,
-                                                "tax": 3.2,
-                                            },
-                                        },
-                                        {
-                                            "summary": "An example with converted data",
-                                            "description": "FastAPI can convert price `strings` to actual `numbers` automatically",
-                                            "value": {"name": "Bar", "price": "35.4"},
+                                            "name": "Foo",
+                                            "description": "A very nice Item",
+                                            "price": 35.4,
+                                            "tax": 3.2,
                                         },
+                                        {"name": "Bar", "price": "35.4"},
                                         {
-                                            "summary": "Invalid data is rejected with an error",
-                                            "value": {
-                                                "name": "Baz",
-                                                "price": "thirty five point four",
-                                            },
+                                            "name": "Baz",
+                                            "price": "thirty five point four",
                                         },
                                     ],
                                 }
                             }
                         },
                         "required": True,
                     },
```

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,38 @@
+import pytest
 from fastapi.testclient import TestClient
 
-from docs_src.schema_extra_example.tutorial004_an import app
+from ...utils import needs_py310
 
-client = TestClient(app)
+
+@pytest.fixture(name="client")
+def get_client():
+    from docs_src.schema_extra_example.tutorial004_an_py310 import app
+
+    client = TestClient(app)
+    return client
 
 
 # Test required and embedded body parameters with no bodies sent
-def test_post_body_example():
+@needs_py310
+def test_post_body_example(client: TestClient):
     response = client.put(
         "/items/5",
         json={
             "name": "Foo",
             "description": "A very nice Item",
             "price": 35.4,
             "tax": 3.2,
         },
     )
     assert response.status_code == 200
 
 
-def test_openapi_schema():
+@needs_py310
+def test_openapi_schema(client: TestClient):
     response = client.get("/openapi.json")
     assert response.status_code == 200, response.text
     assert response.json() == {
         "openapi": "3.1.0",
         "info": {"title": "FastAPI", "version": "0.1.0"},
         "paths": {
             "/items/{item_id}": {
@@ -42,34 +51,23 @@
                         "content": {
                             "application/json": {
                                 "schema": {
                                     "allOf": [{"$ref": "#/components/schemas/Item"}],
                                     "title": "Item",
                                     "examples": [
                                         {
-                                            "summary": "A normal example",
-                                            "description": "A **normal** item works correctly.",
-                                            "value": {
-                                                "name": "Foo",
-                                                "description": "A very nice Item",
-                                                "price": 35.4,
-                                                "tax": 3.2,
-                                            },
-                                        },
-                                        {
-                                            "summary": "An example with converted data",
-                                            "description": "FastAPI can convert price `strings` to actual `numbers` automatically",
-                                            "value": {"name": "Bar", "price": "35.4"},
+                                            "name": "Foo",
+                                            "description": "A very nice Item",
+                                            "price": 35.4,
+                                            "tax": 3.2,
                                         },
+                                        {"name": "Bar", "price": "35.4"},
                                         {
-                                            "summary": "Invalid data is rejected with an error",
-                                            "value": {
-                                                "name": "Baz",
-                                                "price": "thirty five point four",
-                                            },
+                                            "name": "Baz",
+                                            "price": "thirty five point four",
                                         },
                                     ],
                                 }
                             }
                         },
                         "required": True,
                     },
```

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import pytest
 from fastapi.testclient import TestClient
 
-from ...utils import needs_py310
+from ...utils import needs_py39
 
 
 @pytest.fixture(name="client")
 def get_client():
-    from docs_src.schema_extra_example.tutorial004_an_py310 import app
+    from docs_src.schema_extra_example.tutorial004_an_py39 import app
 
     client = TestClient(app)
     return client
 
 
 # Test required and embedded body parameters with no bodies sent
-@needs_py310
+@needs_py39
 def test_post_body_example(client: TestClient):
     response = client.put(
         "/items/5",
         json={
             "name": "Foo",
             "description": "A very nice Item",
             "price": 35.4,
             "tax": 3.2,
         },
     )
     assert response.status_code == 200
 
 
-@needs_py310
+@needs_py39
 def test_openapi_schema(client: TestClient):
     response = client.get("/openapi.json")
     assert response.status_code == 200, response.text
     assert response.json() == {
         "openapi": "3.1.0",
         "info": {"title": "FastAPI", "version": "0.1.0"},
         "paths": {
@@ -51,34 +51,23 @@
                         "content": {
                             "application/json": {
                                 "schema": {
                                     "allOf": [{"$ref": "#/components/schemas/Item"}],
                                     "title": "Item",
                                     "examples": [
                                         {
-                                            "summary": "A normal example",
-                                            "description": "A **normal** item works correctly.",
-                                            "value": {
-                                                "name": "Foo",
-                                                "description": "A very nice Item",
-                                                "price": 35.4,
-                                                "tax": 3.2,
-                                            },
+                                            "name": "Foo",
+                                            "description": "A very nice Item",
+                                            "price": 35.4,
+                                            "tax": 3.2,
                                         },
+                                        {"name": "Bar", "price": "35.4"},
                                         {
-                                            "summary": "An example with converted data",
-                                            "description": "FastAPI can convert price `strings` to actual `numbers` automatically",
-                                            "value": {"name": "Bar", "price": "35.4"},
-                                        },
-                                        {
-                                            "summary": "Invalid data is rejected with an error",
-                                            "value": {
-                                                "name": "Baz",
-                                                "price": "thirty five point four",
-                                            },
+                                            "name": "Baz",
+                                            "price": "thirty five point four",
                                         },
                                     ],
                                 }
                             }
                         },
                         "required": True,
                     },
```

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,29 @@
-import pytest
 from fastapi.testclient import TestClient
 
-from ...utils import needs_py39
+from docs_src.schema_extra_example.tutorial004 import app
 
-
-@pytest.fixture(name="client")
-def get_client():
-    from docs_src.schema_extra_example.tutorial004_an_py39 import app
-
-    client = TestClient(app)
-    return client
+client = TestClient(app)
 
 
 # Test required and embedded body parameters with no bodies sent
-@needs_py39
-def test_post_body_example(client: TestClient):
+def test_post_body_example():
     response = client.put(
         "/items/5",
         json={
             "name": "Foo",
             "description": "A very nice Item",
             "price": 35.4,
             "tax": 3.2,
         },
     )
     assert response.status_code == 200
 
 
-@needs_py39
-def test_openapi_schema(client: TestClient):
+def test_openapi_schema():
     response = client.get("/openapi.json")
     assert response.status_code == 200, response.text
     assert response.json() == {
         "openapi": "3.1.0",
         "info": {"title": "FastAPI", "version": "0.1.0"},
         "paths": {
             "/items/{item_id}": {
@@ -51,34 +42,23 @@
                         "content": {
                             "application/json": {
                                 "schema": {
                                     "allOf": [{"$ref": "#/components/schemas/Item"}],
                                     "title": "Item",
                                     "examples": [
                                         {
-                                            "summary": "A normal example",
-                                            "description": "A **normal** item works correctly.",
-                                            "value": {
-                                                "name": "Foo",
-                                                "description": "A very nice Item",
-                                                "price": 35.4,
-                                                "tax": 3.2,
-                                            },
-                                        },
-                                        {
-                                            "summary": "An example with converted data",
-                                            "description": "FastAPI can convert price `strings` to actual `numbers` automatically",
-                                            "value": {"name": "Bar", "price": "35.4"},
+                                            "name": "Foo",
+                                            "description": "A very nice Item",
+                                            "price": 35.4,
+                                            "tax": 3.2,
                                         },
+                                        {"name": "Bar", "price": "35.4"},
                                         {
-                                            "summary": "Invalid data is rejected with an error",
-                                            "value": {
-                                                "name": "Baz",
-                                                "price": "thirty five point four",
-                                            },
+                                            "name": "Baz",
+                                            "price": "thirty five point four",
                                         },
                                     ],
                                 }
                             }
                         },
                         "required": True,
                     },
```

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_schema_extra_example/test_tutorial004_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_schema_extra_example/test_tutorial004_an.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,29 @@
-import pytest
 from fastapi.testclient import TestClient
 
-from ...utils import needs_py310
+from docs_src.schema_extra_example.tutorial004_an import app
 
-
-@pytest.fixture(name="client")
-def get_client():
-    from docs_src.schema_extra_example.tutorial004_py310 import app
-
-    client = TestClient(app)
-    return client
+client = TestClient(app)
 
 
 # Test required and embedded body parameters with no bodies sent
-@needs_py310
-def test_post_body_example(client: TestClient):
+def test_post_body_example():
     response = client.put(
         "/items/5",
         json={
             "name": "Foo",
             "description": "A very nice Item",
             "price": 35.4,
             "tax": 3.2,
         },
     )
     assert response.status_code == 200
 
 
-@needs_py310
-def test_openapi_schema(client: TestClient):
+def test_openapi_schema():
     response = client.get("/openapi.json")
     assert response.status_code == 200, response.text
     assert response.json() == {
         "openapi": "3.1.0",
         "info": {"title": "FastAPI", "version": "0.1.0"},
         "paths": {
             "/items/{item_id}": {
@@ -51,34 +42,23 @@
                         "content": {
                             "application/json": {
                                 "schema": {
                                     "allOf": [{"$ref": "#/components/schemas/Item"}],
                                     "title": "Item",
                                     "examples": [
                                         {
-                                            "summary": "A normal example",
-                                            "description": "A **normal** item works correctly.",
-                                            "value": {
-                                                "name": "Foo",
-                                                "description": "A very nice Item",
-                                                "price": 35.4,
-                                                "tax": 3.2,
-                                            },
-                                        },
-                                        {
-                                            "summary": "An example with converted data",
-                                            "description": "FastAPI can convert price `strings` to actual `numbers` automatically",
-                                            "value": {"name": "Bar", "price": "35.4"},
+                                            "name": "Foo",
+                                            "description": "A very nice Item",
+                                            "price": 35.4,
+                                            "tax": 3.2,
                                         },
+                                        {"name": "Bar", "price": "35.4"},
                                         {
-                                            "summary": "Invalid data is rejected with an error",
-                                            "value": {
-                                                "name": "Baz",
-                                                "price": "thirty five point four",
-                                            },
+                                            "name": "Baz",
+                                            "price": "thirty five point four",
                                         },
                                     ],
                                 }
                             }
                         },
                         "required": True,
                     },
```

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial001_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial001_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial003.py` & `fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial003_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial003_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial003_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial003_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial003_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial003_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial003_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial005.py` & `fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial005_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial005_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial005_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial005_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial005_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial005_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial005_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial005_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial005_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial006.py` & `fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial006_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_security/test_tutorial006_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_security/test_tutorial006_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_sql_databases/test_sql_databases.py` & `fastapi-0.99.1/tests/test_tutorial/test_sql_databases/test_sql_databases.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py` & `fastapi-0.99.1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_sql_databases/test_sql_databases_middleware_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_sql_databases/test_sql_databases_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_sql_databases/test_sql_databases_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_sql_databases/test_testing_databases.py` & `fastapi-0.99.1/tests/test_tutorial/test_sql_databases/test_testing_databases.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_sql_databases/test_testing_databases_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_sql_databases/test_testing_databases_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_sql_databases_peewee/test_sql_databases_peewee.py` & `fastapi-0.99.1/tests/test_tutorial/test_sql_databases_peewee/test_sql_databases_peewee.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_sub_applications/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_sub_applications/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_templates/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_templates/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_testing/test_main.py` & `fastapi-0.99.1/tests/test_tutorial/test_testing/test_main.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_testing/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_testing/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_testing_dependencies/test_tutorial001_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_websockets/test_tutorial001.py` & `fastapi-0.99.1/tests/test_tutorial/test_websockets/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_websockets/test_tutorial002.py` & `fastapi-0.99.1/tests/test_tutorial/test_websockets/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_websockets/test_tutorial002_an.py` & `fastapi-0.99.1/tests/test_tutorial/test_websockets/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_websockets/test_tutorial002_an_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_websockets/test_tutorial002_an_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_websockets/test_tutorial002_py310.py` & `fastapi-0.99.1/tests/test_tutorial/test_websockets/test_tutorial002_py310.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_websockets/test_tutorial003.py` & `fastapi-0.99.1/tests/test_tutorial/test_websockets/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/tests/test_tutorial/test_websockets/test_tutorial003_py39.py` & `fastapi-0.99.1/tests/test_tutorial/test_websockets/test_tutorial003_py39.py`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/LICENSE` & `fastapi-0.99.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/README.md` & `fastapi-0.99.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/pyproject.toml` & `fastapi-0.99.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi-0.99.0/PKG-INFO` & `fastapi-0.99.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi
-Version: 0.99.0
+Version: 0.99.1
 Summary: FastAPI framework, high performance, easy to learn, fast to code, ready for production
 Project-URL: Homepage, https://github.com/tiangolo/fastapi
 Project-URL: Documentation, https://fastapi.tiangolo.com/
 Project-URL: Repository, https://github.com/tiangolo/fastapi
 Author-email: Sebastián Ramírez <tiangolo@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi Version: 0.99.0 Summary: FastAPI framework,
+Metadata-Version: 2.1 Name: fastapi Version: 0.99.1 Summary: FastAPI framework,
 high performance, easy to learn, fast to code, ready for production Project-
 URL: Homepage, https://github.com/tiangolo/fastapi Project-URL: Documentation,
 https://fastapi.tiangolo.com/ Project-URL: Repository, https://github.com/
 tiangolo/fastapi Author-email: SebastiÃ¡n RamÃ­rez
 gmail.com> License-Expression: MIT License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO Classifier: Framework :: FastAPI Classifier:
```

