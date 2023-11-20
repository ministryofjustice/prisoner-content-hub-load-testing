# Prisoner Content Hub Load Testing

[![repo standards badge](https://img.shields.io/endpoint?labelColor=231f20&color=005ea5&style=for-the-badge&label=MoJ%20Compliant&url=https%3A%2F%2Foperations-engineering-reports.cloud-platform.service.justice.gov.uk%2Fapi%2Fv1%2Fcompliant_public_repositories%2Fendpoint%2Ftemplate-repository&logo=data:image/png;base64,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)](https://operations-engineering-reports.cloud-platform.service.justice.gov.uk/public-report/template-repository)

This repository contains the configuration to run load testing against the Prisoner Content Hub using 
[Apache JMeter](https://jmeter.apache.org/).

The purpose of these tests is to analyse the performance of the system under load in order to provide confidence in 
how far the system can be scaled, and to evaluate code and architectural changes to see if they improve or degrade
system performance.

## Requirements

### Apache JMeter

JMeter is required to run the load testing. It is also useful, though not mandatory, to edit the test configuration 
using JMeter.

Install via brew:

`brew install jmeter`

### Redis & Stunnel

Redis and Stunnel are required if clearing the front end cache prior to running load testing is required.

Install via brew:

`brew install stunnel redis`

## Editing Configuration

Run the JMeter GUI with

`jmeter &`

You should run this command in the root folder of this repository. This is because the output path is specified as a 
relative path, and JMeter treats that as a path relative to from where JMeter was invoked, not relative to the 
JMeter project that you subsequently open.

Once the GUI is running, open the *Content Hub Load Testing.jmx* file in the root of this repository.

Note that whilst you can run the load testing from the GUI, this should only be done for debugging purposes. Accurate
load testing should be done from the command line.

Note as the test configuration .jmx file is am XML file, it can be edited in the IDE or text editor of your choice 
rather than the JMeter  

## Configuration

The bulk of the test configuration is held in the *Content Hub Load Testing.jmx* file.
Additional configuration is held in the CSV files in the data/ folder.

The test uses multiple thread groups, each representing an individual prison. Each thread group loops through the 
paths in *data/common_paths.csv*, which is a set of most commonly used known paths that should return a 200 response 
when issued for any prison. For each, a GET request is issued for that path, for each prison, using the environment 
specified in *data/domain.csv*.

Each thread group also issues search requests at a much lower rate, indicative of the ratio of normal page requests to 
searches. This can be adjusted by adjusting the Throughput value in the Throughput Controller under which the search 
request is nested for each prison's Thread Group. The search terms through which the thread groups loop are listed in 
data/search_terms.csv and are the most common search terms issued on the platform.

All requests will request resources embedded in their respective responses where such resources reside on the same 
domain as the originating request. Resources residing on other domains are not requested. So for example, the CSS,
JS, and favicon may be requested following a page request, but images held on S3 will not. It is not the intention of 
these tests to stress test Amazon S3.

The master throughput of all requests is throttled by the Constant Throughput Timer, which is in the configuration 
before the prison Thread Groups. By default, this is set much lower than production throughput and must be increased to 
perform a representative test. It may also be necessary to adjust the number of threads in each Thread Group to achieve
representative load, and the thread lifetime to match the required test duration.

## Environments

Load tests by default run against the staging environment.

Tests should never be run against the production environment.

To get representative results of expected production system, the staging environment should be temporarily flexed up to 
match production.

This should be done by editing the following files in the https://github.com/ministryofjustice/cloud-platform-environments
repository, and issuing a PR:
* namespaces/live.cloud-platform.service.justice.gov.uk/prisoner-content-hub-staging/02-limitrange.yaml
* namespaces/live.cloud-platform.service.justice.gov.uk/prisoner-content-hub-staging/resources/opensearch.tf
* namespaces/live.cloud-platform.service.justice.gov.uk/prisoner-content-hub-staging/resources/rds.tf

Each has clearly marked sections beginning

> &#8203;# This is the normal setting for staging

or

> &#8203;# These are the normal settings for staging

These should be commented out, and the corresponding sections marked

> &#8203;# These are the settings to flex staging up to match production

or

> &#8203;# This setting is to flex staging up to match production. 

should be uncommented.

**It is vital that these resources are scaled back down as soon as possible to avoid unnecessary AWS costs.**

TODO: add details on clearing caches on front and back end systems.

## Running the Load Testing

### Preparation

If the staging environment has been flexed up, the Drupal search index will need regenerating before running load 
testing at admin/config/search/search-api/index/content_for_search.

Depending on the intention of the test, you may also wish to clear Drupal's cache and the Front End cache.

Drupal's cache can be cleared by running the following command from a prisoner-content-hub-backend pod:

```
drush cache-rebuild; drush cache:force-clear-page
```

The Front End cache is stored in Redis. To clear this cache, you must set up a port forwarding pod to access the Redis
instance referred to by the frontend-redis k8s secret and delete the cache manually.

See https://dsdmoj.atlassian.net/wiki/spaces/HUB/pages/4181262414/Content+Hub+Front+End+Elasticache+Redis for details.

### Execution

Run the load test by issuing the following command from the root of the repository

`jmeter -n -t Content\ Hub\ Load\ Testing.jmx -l output/output.csv -e -o output/html`

Browsable output of the testing will then be available by opening output/html/index.html.
Raw output will be available in output/output.csv.
Application logging will be available in jmeter.log in the root of the repository.

TODO: add info on regenerating the output from a restricted data set.
