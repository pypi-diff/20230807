# Comparing `tmp/getajob-0.6.8.tar.gz` & `tmp/getajob-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getajob-0.6.8.tar", max compression
+gzip compressed data, was "getajob-0.7.0.tar", max compression
```

## Comparing `getajob-0.6.8.tar` & `getajob-0.7.0.tar`

### file list

```diff
@@ -1,218 +1,218 @@
--rw-r--r--   0        0        0    11357 2023-08-06 14:17:05.476462 getajob-0.6.8/LICENSE
--rw-r--r--   0        0        0       69 2023-08-06 14:17:05.480462 getajob-0.6.8/README.md
--rw-r--r--   0        0        0       22 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/__init__.py
--rw-r--r--   0        0        0     3166 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/abstractions/models.py
--rw-r--r--   0        0        0    18136 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/abstractions/repository.py
--rw-r--r--   0        0        0      385 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/abstractions/vendor_client_factory.py
--rw-r--r--   0        0        0     2294 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/config/settings.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/admin/dashboard/__init__.py
--rw-r--r--   0        0        0      160 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/admin/dashboard/models.py
--rw-r--r--   0        0        0      353 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/admin/dashboard/repository.py
--rw-r--r--   0        0        0     1209 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/admin/dashboard/unit_of_work.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/admin/search/__init__.py
--rw-r--r--   0        0        0      141 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/admin/search/models.py
--rw-r--r--   0        0        0      631 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/admin/search/repository.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/admin/users/__init__.py
--rw-r--r--   0        0        0      620 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/admin/users/models.py
--rw-r--r--   0        0        0      844 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/admin/users/repository.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/applications/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/applications/applicant_tracking/__init__.py
--rw-r--r--   0        0        0     1044 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/applications/applicant_tracking/models.py
--rw-r--r--   0        0        0     2502 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/applications/applicant_tracking/repository.py
--rw-r--r--   0        0        0     4438 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/applications/async_service.py
--rw-r--r--   0        0        0      277 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/applications/enumerations.py
--rw-r--r--   0        0        0     1851 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/applications/models.py
--rw-r--r--   0        0        0     3804 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/applications/repository.py
--rw-r--r--   0        0        0     1781 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/applications/search.py
--rw-r--r--   0        0        0     2629 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/applications/unit_of_work.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/chat/__init__.py
--rw-r--r--   0        0        0     2617 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/chat/async_service.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/chat/message/__init__.py
--rw-r--r--   0        0        0      616 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/chat/message/models.py
--rw-r--r--   0        0        0      892 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/chat/message/repository.py
--rw-r--r--   0        0        0      272 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/chat/models.py
--rw-r--r--   0        0        0     1899 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/chat/repository.py
--rw-r--r--   0        0        0     1650 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/chat/unit_of_work.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/applicant_tracking_settings/__init__.py
--rw-r--r--   0        0        0      531 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/applicant_tracking_settings/models.py
--rw-r--r--   0        0        0     1086 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/applicant_tracking_settings/repository.py
--rw-r--r--   0        0        0      175 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/applicant_tracking_settings/unit_of_work.py
--rw-r--r--   0        0        0     2375 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/async_service.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/audit/__init__.py
--rw-r--r--   0        0        0     2100 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/audit/async_service.py
--rw-r--r--   0        0        0      482 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/audit/models.py
--rw-r--r--   0        0        0     1104 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/audit/repository.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/dashboard/__init__.py
--rw-r--r--   0        0        0      145 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/dashboard/models.py
--rw-r--r--   0        0        0      861 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/dashboard/repository.py
--rw-r--r--   0        0        0     1727 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/dashboard/unit_of_work.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/details/__init__.py
--rw-r--r--   0        0        0      713 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/details/models.py
--rw-r--r--   0        0        0     1448 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/details/repository.py
--rw-r--r--   0        0        0     2243 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/enumerations.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/invitations/__init__.py
--rw-r--r--   0        0        0      145 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/invitations/models.py
--rw-r--r--   0        0        0      786 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/invitations/repository.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/job_templates/__init__.py
--rw-r--r--   0        0        0     1644 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/job_templates/models.py
--rw-r--r--   0        0        0      862 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/job_templates/repository.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/jobs/__init__.py
--rw-r--r--   0        0        0     3865 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/jobs/async_service.py
--rw-r--r--   0        0        0     3641 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/jobs/models.py
--rw-r--r--   0        0        0     1421 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/jobs/repository.py
--rw-r--r--   0        0        0      533 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/jobs/unit_of_work.py
--rw-r--r--   0        0        0      102 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/models.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/recruiters/__init__.py
--rw-r--r--   0        0        0      117 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/recruiters/models.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/recruiters/recruiter_settings/__init__.py
--rw-r--r--   0        0        0      387 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/recruiters/recruiter_settings/models.py
--rw-r--r--   0        0        0      958 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/recruiters/recruiter_settings/repository.py
--rw-r--r--   0        0        0      744 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/recruiters/repository.py
--rw-r--r--   0        0        0     1357 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/repository.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/saved_candidates/__init__.py
--rw-r--r--   0        0        0      323 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/saved_candidates/models.py
--rw-r--r--   0        0        0     2287 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/companies/saved_candidates/repository.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/scheduled_events/__init__.py
--rw-r--r--   0        0        0      210 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/scheduled_events/enumerations.py
--rw-r--r--   0        0        0      995 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/scheduled_events/models.py
--rw-r--r--   0        0        0     1865 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/scheduled_events/repository.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/search/__init__.py
--rw-r--r--   0        0        0     1732 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/search/models.py
--rw-r--r--   0        0        0     5410 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/async_service.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/cover_letters/__init__.py
--rw-r--r--   0        0        0      277 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/cover_letters/models.py
--rw-r--r--   0        0        0      854 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/cover_letters/repository.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/dashboard/__init__.py
--rw-r--r--   0        0        0      115 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/dashboard/models.py
--rw-r--r--   0        0        0      661 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/dashboard/repository.py
--rw-r--r--   0        0        0     1202 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/dashboard/unit_of_work.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/details/__init__.py
--rw-r--r--   0        0        0     2974 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/details/models.py
--rw-r--r--   0        0        0     1416 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/details/repository.py
--rw-r--r--   0        0        0     1213 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/enumerations.py
--rw-r--r--   0        0        0       89 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/models.py
--rw-r--r--   0        0        0     1362 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/repository.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/extracted_data/__init__.py
--rw-r--r--   0        0        0     7480 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/extracted_data/extractor.py
--rw-r--r--   0        0        0     1966 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/extracted_data/models.py
--rw-r--r--   0        0        0     1449 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/extracted_data/repository.py
--rw-r--r--   0        0        0      988 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/extracted_data/unit_of_work.py
--rw-r--r--   0        0        0      402 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/models.py
--rw-r--r--   0        0        0     1707 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/repository.py
--rw-r--r--   0        0        0     2649 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_10-10.pdf.json
--rw-r--r--   0        0        0     3412 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_11-11.pdf.json
--rw-r--r--   0        0        0     1591 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_12-12.pdf.json
--rw-r--r--   0        0        0     4311 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_13-end.pdf.json
--rw-r--r--   0        0        0     2018 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_2-2.pdf.json
--rw-r--r--   0        0        0     2479 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_3-3.pdf.json
--rw-r--r--   0        0        0     2333 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_4-4.pdf.json
--rw-r--r--   0        0        0     1844 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_5-5.pdf.json
--rw-r--r--   0        0        0     4264 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_6-6.pdf.json
--rw-r--r--   0        0        0     1806 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_7-7.pdf.json
--rw-r--r--   0        0        0     2523 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_8-8.pdf.json
--rw-r--r--   0        0        0     2028 2023-08-06 14:17:05.480462 getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_9-9.pdf.json
--rw-r--r--   0        0        0   107453 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_10-10.pdf
--rw-r--r--   0        0        0   173006 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_11-11.pdf
--rw-r--r--   0        0        0   107503 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_12-12.pdf
--rw-r--r--   0        0        0   111154 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_13-end.pdf
--rw-r--r--   0        0        0   107645 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_2-2.pdf
--rw-r--r--   0        0        0    30834 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_3-3.pdf
--rw-r--r--   0        0        0    30608 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_4-4.pdf
--rw-r--r--   0        0        0    31147 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_5-5.pdf
--rw-r--r--   0        0        0   107907 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_6-6.pdf
--rw-r--r--   0        0        0   106257 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_7-7.pdf
--rw-r--r--   0        0        0   121496 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_8-8.pdf
--rw-r--r--   0        0        0   106308 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_9-9.pdf
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/resumes/suggestions/__init__.py
--rw-r--r--   0        0        0      701 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/resumes/suggestions/repository.py
--rw-r--r--   0        0        0      459 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/resumes/suggestions/suggestor.py
--rw-r--r--   0        0        0      874 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/resumes/suggestions/unit_of_work.py
--rw-r--r--   0        0        0     2628 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/resumes/unt_of_work.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/saved_jobs/__init__.py
--rw-r--r--   0        0        0      284 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/saved_jobs/models.py
--rw-r--r--   0        0        0     2774 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/saved_jobs/repository.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/sessions/__init__.py
--rw-r--r--   0        0        0      481 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/contexts/users/sessions/models.py
--rw-r--r--   0        0        0     3089 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/exceptions.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/static/__init__.py
--rw-r--r--   0        0        0     1518 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/static/enumerations.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/test_support/__init__.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/test_support/fixtures/__init__.py
--rw-r--r--   0        0        0     2286 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/test_support/fixtures/application.py
--rw-r--r--   0        0        0     1750 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/test_support/fixtures/chat.py
--rw-r--r--   0        0        0     1027 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/test_support/fixtures/company.py
--rw-r--r--   0        0        0      408 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/test_support/fixtures/job.py
--rw-r--r--   0        0        0     1843 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/test_support/fixtures/recruiter.py
--rw-r--r--   0        0        0      645 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/test_support/fixtures/recruiter_invitation.py
--rw-r--r--   0        0        0     1720 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/test_support/fixtures/scheduled_events.py
--rw-r--r--   0        0        0     2579 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/test_support/fixtures/users.py
--rw-r--r--   0        0        0     1861 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/utils.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/vendor/__init__.py
--rw-r--r--   0        0        0      165 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/vendor/aiocron.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/vendor/algolia/__init__.py
--rw-r--r--   0        0        0      468 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/vendor/algolia/client_factory.py
--rw-r--r--   0        0        0     2359 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/vendor/algolia/mock.py
--rw-r--r--   0        0        0      758 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/vendor/algolia/models.py
--rw-r--r--   0        0        0     2656 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/vendor/algolia/repository.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/vendor/clerk/__init__.py
--rw-r--r--   0        0        0     2139 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/vendor/clerk/client.py
--rw-r--r--   0        0        0      340 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/vendor/clerk/client_factory.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/vendor/clerk/companies/__init__.py
--rw-r--r--   0        0        0      894 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/vendor/clerk/companies/models.py
--rw-r--r--   0        0        0     2427 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/vendor/clerk/companies/repository.py
--rw-r--r--   0        0        0     1735 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/vendor/clerk/companies/unit_of_work.py
--rw-r--r--   0        0        0     2553 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/vendor/clerk/mock.py
--rw-r--r--   0        0        0      413 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/vendor/clerk/models.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/vendor/clerk/recruiter_invitation/__init__.py
--rw-r--r--   0        0        0      747 2023-08-06 14:17:05.484462 getajob-0.6.8/getajob/vendor/clerk/recruiter_invitation/models.py
--rw-r--r--   0        0        0     2057 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/clerk/recruiter_invitation/repository.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/clerk/recruiters/__init__.py
--rw-r--r--   0        0        0     1588 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/clerk/recruiters/models.py
--rw-r--r--   0        0        0     3215 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/clerk/recruiters/repository.py
--rw-r--r--   0        0        0     2318 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/clerk/repository.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/clerk/users/__init__.py
--rw-r--r--   0        0        0     1353 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/clerk/users/models.py
--rw-r--r--   0        0        0     2702 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/clerk/users/repository.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/firebase_storage/__init__.py
--rw-r--r--   0        0        0      846 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/firebase_storage/client_factory.py
--rw-r--r--   0        0        0      953 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/firebase_storage/mock.py
--rw-r--r--   0        0        0     1727 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/firebase_storage/repository.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/firestore/__init__.py
--rw-r--r--   0        0        0      749 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/firestore/client_factory.py
--rw-r--r--   0        0        0     1102 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/firestore/helpers.py
--rw-r--r--   0        0        0      507 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/firestore/mock.py
--rw-r--r--   0        0        0     1975 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/firestore/models.py
--rw-r--r--   0        0        0    11165 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/firestore/repository.py
--rw-r--r--   0        0        0      696 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/jwt.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/kafka/__init__.py
--rw-r--r--   0        0        0     1721 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/kafka/client_factory.py
--rw-r--r--   0        0        0      716 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/kafka/mock.py
--rw-r--r--   0        0        0     2297 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/kafka/models.py
--rw-r--r--   0        0        0     1342 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/kafka/repository.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/mailgun/__init__.py
--rw-r--r--   0        0        0      989 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/mailgun/client_factory.py
--rw-r--r--   0        0        0      282 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/mailgun/mock.py
--rw-r--r--   0        0        0     1231 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/mailgun/repository.py
--rw-r--r--   0        0        0      104 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/mailgun/templates/chat_message.html
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/openai/__init__.py
--rw-r--r--   0        0        0      447 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/openai/client_factory.py
--rw-r--r--   0        0        0      521 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/openai/mock.py
--rw-r--r--   0        0        0     1185 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/openai/repository.py
--rw-r--r--   0        0        0      572 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/openai/settings.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/qstash/__init__.py
--rw-r--r--   0        0        0     2148 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/qstash/client.py
--rw-r--r--   0        0        0      332 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/qstash/client_factory.py
--rw-r--r--   0        0        0      214 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/qstash/mock.py
--rw-r--r--   0        0        0      276 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/qstash/models.py
--rw-r--r--   0        0        0      649 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/qstash/repository.py
--rw-r--r--   0        0        0        0 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/redis/__init__.py
--rw-r--r--   0        0        0      508 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/redis/client_factory.py
--rw-r--r--   0        0        0      343 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/redis/mock.py
--rw-r--r--   0        0        0     2463 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/redis/repository.py
--rw-r--r--   0        0        0      251 2023-08-06 14:17:05.488462 getajob-0.6.8/getajob/vendor/sentry.py
--rw-r--r--   0        0        0     1809 2023-08-06 14:17:05.488462 getajob-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     2937 1970-01-01 00:00:00.000000 getajob-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-07 18:39:13.391114 getajob-0.7.0/LICENSE
+-rw-r--r--   0        0        0       69 2023-08-07 18:39:13.395114 getajob-0.7.0/README.md
+-rw-r--r--   0        0        0       22 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/__init__.py
+-rw-r--r--   0        0        0     3166 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/abstractions/models.py
+-rw-r--r--   0        0        0    18136 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/abstractions/repository.py
+-rw-r--r--   0        0        0      385 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/abstractions/vendor_client_factory.py
+-rw-r--r--   0        0        0     2294 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/config/settings.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/admin/dashboard/__init__.py
+-rw-r--r--   0        0        0      160 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/admin/dashboard/models.py
+-rw-r--r--   0        0        0      353 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/admin/dashboard/repository.py
+-rw-r--r--   0        0        0     1209 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/admin/dashboard/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/admin/search/__init__.py
+-rw-r--r--   0        0        0      141 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/admin/search/models.py
+-rw-r--r--   0        0        0      631 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/admin/search/repository.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/admin/users/__init__.py
+-rw-r--r--   0        0        0      620 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/admin/users/models.py
+-rw-r--r--   0        0        0      844 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/admin/users/repository.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/applications/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/applications/applicant_tracking/__init__.py
+-rw-r--r--   0        0        0     1044 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/applications/applicant_tracking/models.py
+-rw-r--r--   0        0        0     2502 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/applications/applicant_tracking/repository.py
+-rw-r--r--   0        0        0     4438 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/applications/async_service.py
+-rw-r--r--   0        0        0      277 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/applications/enumerations.py
+-rw-r--r--   0        0        0     1851 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/applications/models.py
+-rw-r--r--   0        0        0     3804 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/applications/repository.py
+-rw-r--r--   0        0        0     1781 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/applications/search.py
+-rw-r--r--   0        0        0     2629 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/applications/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/chat/__init__.py
+-rw-r--r--   0        0        0     2617 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/chat/async_service.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/chat/message/__init__.py
+-rw-r--r--   0        0        0      616 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/chat/message/models.py
+-rw-r--r--   0        0        0      892 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/chat/message/repository.py
+-rw-r--r--   0        0        0      272 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/chat/models.py
+-rw-r--r--   0        0        0     1899 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/chat/repository.py
+-rw-r--r--   0        0        0     1650 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/chat/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/applicant_tracking_settings/__init__.py
+-rw-r--r--   0        0        0      531 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/applicant_tracking_settings/models.py
+-rw-r--r--   0        0        0     1086 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/applicant_tracking_settings/repository.py
+-rw-r--r--   0        0        0      175 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/applicant_tracking_settings/unit_of_work.py
+-rw-r--r--   0        0        0     2375 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/async_service.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/audit/__init__.py
+-rw-r--r--   0        0        0     2100 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/audit/async_service.py
+-rw-r--r--   0        0        0      482 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/audit/models.py
+-rw-r--r--   0        0        0     1104 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/audit/repository.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/dashboard/__init__.py
+-rw-r--r--   0        0        0      145 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/dashboard/models.py
+-rw-r--r--   0        0        0      861 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/dashboard/repository.py
+-rw-r--r--   0        0        0     1727 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/dashboard/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/details/__init__.py
+-rw-r--r--   0        0        0      713 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/details/models.py
+-rw-r--r--   0        0        0     1448 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/details/repository.py
+-rw-r--r--   0        0        0     2243 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/enumerations.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/invitations/__init__.py
+-rw-r--r--   0        0        0      145 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/invitations/models.py
+-rw-r--r--   0        0        0      786 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/invitations/repository.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/job_templates/__init__.py
+-rw-r--r--   0        0        0     1644 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/job_templates/models.py
+-rw-r--r--   0        0        0      862 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/job_templates/repository.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/jobs/__init__.py
+-rw-r--r--   0        0        0     3311 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/jobs/async_service.py
+-rw-r--r--   0        0        0     3641 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/jobs/models.py
+-rw-r--r--   0        0        0     1421 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/jobs/repository.py
+-rw-r--r--   0        0        0      533 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/jobs/unit_of_work.py
+-rw-r--r--   0        0        0      102 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/models.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/recruiters/__init__.py
+-rw-r--r--   0        0        0      117 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/recruiters/models.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/recruiters/recruiter_settings/__init__.py
+-rw-r--r--   0        0        0      387 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/recruiters/recruiter_settings/models.py
+-rw-r--r--   0        0        0      958 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/recruiters/recruiter_settings/repository.py
+-rw-r--r--   0        0        0      744 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/recruiters/repository.py
+-rw-r--r--   0        0        0     1357 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/repository.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/saved_candidates/__init__.py
+-rw-r--r--   0        0        0      323 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/saved_candidates/models.py
+-rw-r--r--   0        0        0     2287 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/companies/saved_candidates/repository.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/scheduled_events/__init__.py
+-rw-r--r--   0        0        0      210 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/scheduled_events/enumerations.py
+-rw-r--r--   0        0        0      995 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/scheduled_events/models.py
+-rw-r--r--   0        0        0     1865 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/scheduled_events/repository.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/search/__init__.py
+-rw-r--r--   0        0        0     1732 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/search/models.py
+-rw-r--r--   0        0        0     4302 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/users/async_service.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/users/cover_letters/__init__.py
+-rw-r--r--   0        0        0      277 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/users/cover_letters/models.py
+-rw-r--r--   0        0        0      854 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/users/cover_letters/repository.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/users/dashboard/__init__.py
+-rw-r--r--   0        0        0      115 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/users/dashboard/models.py
+-rw-r--r--   0        0        0      661 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/users/dashboard/repository.py
+-rw-r--r--   0        0        0     1202 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/users/dashboard/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/users/details/__init__.py
+-rw-r--r--   0        0        0     2974 2023-08-07 18:39:13.395114 getajob-0.7.0/getajob/contexts/users/details/models.py
+-rw-r--r--   0        0        0     1416 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/details/repository.py
+-rw-r--r--   0        0        0     1213 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/enumerations.py
+-rw-r--r--   0        0        0       89 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/models.py
+-rw-r--r--   0        0        0     1362 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/repository.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/extracted_data/__init__.py
+-rw-r--r--   0        0        0     7480 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/extracted_data/extractor.py
+-rw-r--r--   0        0        0     1966 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/extracted_data/models.py
+-rw-r--r--   0        0        0     1449 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/extracted_data/repository.py
+-rw-r--r--   0        0        0      988 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/extracted_data/unit_of_work.py
+-rw-r--r--   0        0        0      402 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/models.py
+-rw-r--r--   0        0        0     1707 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/repository.py
+-rw-r--r--   0        0        0     2649 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_10-10.pdf.json
+-rw-r--r--   0        0        0     3412 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_11-11.pdf.json
+-rw-r--r--   0        0        0     1591 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_12-12.pdf.json
+-rw-r--r--   0        0        0     4311 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_13-end.pdf.json
+-rw-r--r--   0        0        0     2018 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_2-2.pdf.json
+-rw-r--r--   0        0        0     2479 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_3-3.pdf.json
+-rw-r--r--   0        0        0     2333 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_4-4.pdf.json
+-rw-r--r--   0        0        0     1844 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_5-5.pdf.json
+-rw-r--r--   0        0        0     4264 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_6-6.pdf.json
+-rw-r--r--   0        0        0     1806 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_7-7.pdf.json
+-rw-r--r--   0        0        0     2523 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_8-8.pdf.json
+-rw-r--r--   0        0        0     2028 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_9-9.pdf.json
+-rw-r--r--   0        0        0   107453 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_10-10.pdf
+-rw-r--r--   0        0        0   173006 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_11-11.pdf
+-rw-r--r--   0        0        0   107503 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_12-12.pdf
+-rw-r--r--   0        0        0   111154 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_13-end.pdf
+-rw-r--r--   0        0        0   107645 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_2-2.pdf
+-rw-r--r--   0        0        0    30834 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_3-3.pdf
+-rw-r--r--   0        0        0    30608 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_4-4.pdf
+-rw-r--r--   0        0        0    31147 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_5-5.pdf
+-rw-r--r--   0        0        0   107907 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_6-6.pdf
+-rw-r--r--   0        0        0   106257 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_7-7.pdf
+-rw-r--r--   0        0        0   121496 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_8-8.pdf
+-rw-r--r--   0        0        0   106308 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_9-9.pdf
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/suggestions/__init__.py
+-rw-r--r--   0        0        0      701 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/suggestions/repository.py
+-rw-r--r--   0        0        0      459 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/suggestions/suggestor.py
+-rw-r--r--   0        0        0      874 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/suggestions/unit_of_work.py
+-rw-r--r--   0        0        0     2628 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/resumes/unt_of_work.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/saved_jobs/__init__.py
+-rw-r--r--   0        0        0      284 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/saved_jobs/models.py
+-rw-r--r--   0        0        0     2774 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/saved_jobs/repository.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/sessions/__init__.py
+-rw-r--r--   0        0        0      481 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/contexts/users/sessions/models.py
+-rw-r--r--   0        0        0     3089 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/exceptions.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/static/__init__.py
+-rw-r--r--   0        0        0     1518 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/static/enumerations.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.399114 getajob-0.7.0/getajob/test_support/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/test_support/fixtures/__init__.py
+-rw-r--r--   0        0        0     2286 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/test_support/fixtures/application.py
+-rw-r--r--   0        0        0     1750 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/test_support/fixtures/chat.py
+-rw-r--r--   0        0        0     1027 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/test_support/fixtures/company.py
+-rw-r--r--   0        0        0      408 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/test_support/fixtures/job.py
+-rw-r--r--   0        0        0     1843 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/test_support/fixtures/recruiter.py
+-rw-r--r--   0        0        0      645 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/test_support/fixtures/recruiter_invitation.py
+-rw-r--r--   0        0        0     1720 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/test_support/fixtures/scheduled_events.py
+-rw-r--r--   0        0        0     2579 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/test_support/fixtures/users.py
+-rw-r--r--   0        0        0     1861 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/utils.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/__init__.py
+-rw-r--r--   0        0        0      165 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/aiocron.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/algolia/__init__.py
+-rw-r--r--   0        0        0      468 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/algolia/client_factory.py
+-rw-r--r--   0        0        0     2359 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/algolia/mock.py
+-rw-r--r--   0        0        0      758 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/algolia/models.py
+-rw-r--r--   0        0        0     2656 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/algolia/repository.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/clerk/__init__.py
+-rw-r--r--   0        0        0     2139 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/clerk/client.py
+-rw-r--r--   0        0        0      340 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/clerk/client_factory.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/clerk/companies/__init__.py
+-rw-r--r--   0        0        0      894 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/clerk/companies/models.py
+-rw-r--r--   0        0        0     2427 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/clerk/companies/repository.py
+-rw-r--r--   0        0        0     1735 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/clerk/companies/unit_of_work.py
+-rw-r--r--   0        0        0     2553 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/clerk/mock.py
+-rw-r--r--   0        0        0      413 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/clerk/models.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/clerk/recruiter_invitation/__init__.py
+-rw-r--r--   0        0        0      747 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/clerk/recruiter_invitation/models.py
+-rw-r--r--   0        0        0     2057 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/clerk/recruiter_invitation/repository.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/clerk/recruiters/__init__.py
+-rw-r--r--   0        0        0     1588 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/clerk/recruiters/models.py
+-rw-r--r--   0        0        0     3215 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/clerk/recruiters/repository.py
+-rw-r--r--   0        0        0     2318 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/clerk/repository.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/clerk/users/__init__.py
+-rw-r--r--   0        0        0     1353 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/clerk/users/models.py
+-rw-r--r--   0        0        0     2702 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/clerk/users/repository.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/firebase_storage/__init__.py
+-rw-r--r--   0        0        0      846 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/firebase_storage/client_factory.py
+-rw-r--r--   0        0        0      953 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/firebase_storage/mock.py
+-rw-r--r--   0        0        0     1727 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/firebase_storage/repository.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/firestore/__init__.py
+-rw-r--r--   0        0        0      749 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/firestore/client_factory.py
+-rw-r--r--   0        0        0     1102 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/firestore/helpers.py
+-rw-r--r--   0        0        0      507 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/firestore/mock.py
+-rw-r--r--   0        0        0     1975 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/firestore/models.py
+-rw-r--r--   0        0        0    11165 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/firestore/repository.py
+-rw-r--r--   0        0        0      696 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/jwt.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/kafka/__init__.py
+-rw-r--r--   0        0        0     1721 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/kafka/client_factory.py
+-rw-r--r--   0        0        0      716 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/kafka/mock.py
+-rw-r--r--   0        0        0     2984 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/kafka/models.py
+-rw-r--r--   0        0        0     1464 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/kafka/repository.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/mailgun/__init__.py
+-rw-r--r--   0        0        0      989 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/mailgun/client_factory.py
+-rw-r--r--   0        0        0      282 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/mailgun/mock.py
+-rw-r--r--   0        0        0     1231 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/mailgun/repository.py
+-rw-r--r--   0        0        0      104 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/mailgun/templates/chat_message.html
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/openai/__init__.py
+-rw-r--r--   0        0        0      447 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/openai/client_factory.py
+-rw-r--r--   0        0        0      521 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/openai/mock.py
+-rw-r--r--   0        0        0     1185 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/openai/repository.py
+-rw-r--r--   0        0        0      572 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/openai/settings.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/qstash/__init__.py
+-rw-r--r--   0        0        0     2148 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/qstash/client.py
+-rw-r--r--   0        0        0      332 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/qstash/client_factory.py
+-rw-r--r--   0        0        0      214 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/qstash/mock.py
+-rw-r--r--   0        0        0      276 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/qstash/models.py
+-rw-r--r--   0        0        0      649 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/qstash/repository.py
+-rw-r--r--   0        0        0        0 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/redis/__init__.py
+-rw-r--r--   0        0        0      508 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/redis/client_factory.py
+-rw-r--r--   0        0        0      343 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/redis/mock.py
+-rw-r--r--   0        0        0     2463 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/redis/repository.py
+-rw-r--r--   0        0        0      251 2023-08-07 18:39:13.403114 getajob-0.7.0/getajob/vendor/sentry.py
+-rw-r--r--   0        0        0     1809 2023-08-07 18:39:13.403114 getajob-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2937 1970-01-01 00:00:00.000000 getajob-0.7.0/PKG-INFO
```

### Comparing `getajob-0.6.8/LICENSE` & `getajob-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/abstractions/models.py` & `getajob-0.7.0/getajob/abstractions/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/abstractions/repository.py` & `getajob-0.7.0/getajob/abstractions/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/config/settings.py` & `getajob-0.7.0/getajob/config/settings.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/admin/dashboard/unit_of_work.py` & `getajob-0.7.0/getajob/contexts/admin/dashboard/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/admin/search/repository.py` & `getajob-0.7.0/getajob/contexts/admin/search/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/admin/users/models.py` & `getajob-0.7.0/getajob/contexts/admin/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/admin/users/repository.py` & `getajob-0.7.0/getajob/contexts/admin/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/applications/applicant_tracking/models.py` & `getajob-0.7.0/getajob/contexts/applications/applicant_tracking/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/applications/applicant_tracking/repository.py` & `getajob-0.7.0/getajob/contexts/applications/applicant_tracking/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/applications/async_service.py` & `getajob-0.7.0/getajob/contexts/applications/async_service.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/applications/models.py` & `getajob-0.7.0/getajob/contexts/applications/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/applications/repository.py` & `getajob-0.7.0/getajob/contexts/applications/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/applications/search.py` & `getajob-0.7.0/getajob/contexts/applications/search.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/applications/unit_of_work.py` & `getajob-0.7.0/getajob/contexts/applications/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/chat/async_service.py` & `getajob-0.7.0/getajob/contexts/chat/async_service.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/chat/message/models.py` & `getajob-0.7.0/getajob/contexts/chat/message/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/chat/message/repository.py` & `getajob-0.7.0/getajob/contexts/chat/message/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/chat/repository.py` & `getajob-0.7.0/getajob/contexts/chat/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/chat/unit_of_work.py` & `getajob-0.7.0/getajob/contexts/chat/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/applicant_tracking_settings/models.py` & `getajob-0.7.0/getajob/contexts/companies/applicant_tracking_settings/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/applicant_tracking_settings/repository.py` & `getajob-0.7.0/getajob/contexts/companies/applicant_tracking_settings/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/async_service.py` & `getajob-0.7.0/getajob/contexts/companies/async_service.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/audit/async_service.py` & `getajob-0.7.0/getajob/contexts/companies/audit/async_service.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/audit/repository.py` & `getajob-0.7.0/getajob/contexts/companies/audit/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/dashboard/repository.py` & `getajob-0.7.0/getajob/contexts/companies/dashboard/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/dashboard/unit_of_work.py` & `getajob-0.7.0/getajob/contexts/companies/dashboard/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/details/models.py` & `getajob-0.7.0/getajob/contexts/companies/details/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/details/repository.py` & `getajob-0.7.0/getajob/contexts/companies/details/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/enumerations.py` & `getajob-0.7.0/getajob/contexts/companies/enumerations.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/invitations/repository.py` & `getajob-0.7.0/getajob/contexts/companies/invitations/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/job_templates/models.py` & `getajob-0.7.0/getajob/contexts/companies/job_templates/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/job_templates/repository.py` & `getajob-0.7.0/getajob/contexts/companies/job_templates/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/jobs/async_service.py` & `getajob-0.7.0/getajob/contexts/companies/jobs/async_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,29 +17,14 @@
         self,
         algolia_jobs: AlgoliaSearchRepository,
         algolia_applications: AlgoliaSearchRepository,
     ):
         self.algolia_jobs = algolia_jobs
         self.algolia_applications = algolia_applications
 
-    async def get_job(self, processed_message: ProcessedKafkaMessage):
-        job_data = cast(Job, processed_message.data)
-        job_repo = JobsRepository(
-            request_scope=processed_message.request_scope, kafka=None
-        )
-        job_repo.update(
-            job_data.id,
-            InternalUpdateJob(view_count=job_data.view_count + 1),
-            parent_collections={
-                Entity.COMPANIES.value: processed_message.parent_collections[
-                    Entity.COMPANIES.value
-                ]
-            },
-        )
-
     async def create_job(self, processed_message: ProcessedKafkaMessage):
         job_data = cast(Job, processed_message.data)
         self.algolia_jobs.create_object(
             object_id=job_data.id,
             object_data=JobSearch(
                 id=job_data.id,
                 created=datetime.now(),
```

### Comparing `getajob-0.6.8/getajob/contexts/companies/jobs/models.py` & `getajob-0.7.0/getajob/contexts/companies/jobs/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/jobs/repository.py` & `getajob-0.7.0/getajob/contexts/companies/jobs/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/jobs/unit_of_work.py` & `getajob-0.7.0/getajob/contexts/companies/jobs/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/recruiters/recruiter_settings/repository.py` & `getajob-0.7.0/getajob/contexts/companies/recruiters/recruiter_settings/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/recruiters/repository.py` & `getajob-0.7.0/getajob/contexts/companies/recruiters/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/repository.py` & `getajob-0.7.0/getajob/contexts/companies/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/companies/saved_candidates/repository.py` & `getajob-0.7.0/getajob/contexts/companies/saved_candidates/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/scheduled_events/models.py` & `getajob-0.7.0/getajob/contexts/scheduled_events/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/scheduled_events/repository.py` & `getajob-0.7.0/getajob/contexts/scheduled_events/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/search/models.py` & `getajob-0.7.0/getajob/contexts/search/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/cover_letters/repository.py` & `getajob-0.7.0/getajob/contexts/users/cover_letters/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/dashboard/repository.py` & `getajob-0.7.0/getajob/contexts/users/dashboard/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/dashboard/unit_of_work.py` & `getajob-0.7.0/getajob/contexts/users/dashboard/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/details/models.py` & `getajob-0.7.0/getajob/contexts/users/details/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/details/repository.py` & `getajob-0.7.0/getajob/contexts/users/details/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/enumerations.py` & `getajob-0.7.0/getajob/contexts/users/enumerations.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/repository.py` & `getajob-0.7.0/getajob/contexts/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/extracted_data/extractor.py` & `getajob-0.7.0/getajob/contexts/users/resumes/extracted_data/extractor.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/extracted_data/models.py` & `getajob-0.7.0/getajob/contexts/users/resumes/extracted_data/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/extracted_data/repository.py` & `getajob-0.7.0/getajob/contexts/users/resumes/extracted_data/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/extracted_data/unit_of_work.py` & `getajob-0.7.0/getajob/contexts/users/resumes/extracted_data/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/repository.py` & `getajob-0.7.0/getajob/contexts/users/resumes/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_10-10.pdf.json` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_10-10.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_11-11.pdf.json` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_11-11.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_12-12.pdf.json` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_12-12.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_13-end.pdf.json` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_13-end.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_2-2.pdf.json` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_2-2.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_3-3.pdf.json` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_3-3.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_4-4.pdf.json` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_4-4.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_5-5.pdf.json` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_5-5.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_6-6.pdf.json` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_6-6.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_7-7.pdf.json` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_7-7.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_8-8.pdf.json` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_8-8.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/extracted_resume-samples_9-9.pdf.json` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/extracted_resume-samples_9-9.pdf.json`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_10-10.pdf` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_10-10.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_11-11.pdf` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_11-11.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_12-12.pdf` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_12-12.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_13-end.pdf` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_13-end.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_2-2.pdf` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_2-2.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_3-3.pdf` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_3-3.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_4-4.pdf` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_4-4.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_5-5.pdf` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_5-5.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_6-6.pdf` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_6-6.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_7-7.pdf` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_7-7.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_8-8.pdf` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_8-8.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/samples/resume-samples_9-9.pdf` & `getajob-0.7.0/getajob/contexts/users/resumes/samples/resume-samples_9-9.pdf`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/suggestions/repository.py` & `getajob-0.7.0/getajob/contexts/users/resumes/suggestions/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/suggestions/unit_of_work.py` & `getajob-0.7.0/getajob/contexts/users/resumes/suggestions/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/resumes/unt_of_work.py` & `getajob-0.7.0/getajob/contexts/users/resumes/unt_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/contexts/users/saved_jobs/repository.py` & `getajob-0.7.0/getajob/contexts/users/saved_jobs/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/exceptions.py` & `getajob-0.7.0/getajob/exceptions.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/static/enumerations.py` & `getajob-0.7.0/getajob/static/enumerations.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/test_support/fixtures/application.py` & `getajob-0.7.0/getajob/test_support/fixtures/application.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/test_support/fixtures/chat.py` & `getajob-0.7.0/getajob/test_support/fixtures/chat.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/test_support/fixtures/company.py` & `getajob-0.7.0/getajob/test_support/fixtures/company.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/test_support/fixtures/recruiter.py` & `getajob-0.7.0/getajob/test_support/fixtures/recruiter.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/test_support/fixtures/recruiter_invitation.py` & `getajob-0.7.0/getajob/test_support/fixtures/recruiter_invitation.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/test_support/fixtures/scheduled_events.py` & `getajob-0.7.0/getajob/test_support/fixtures/scheduled_events.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/test_support/fixtures/users.py` & `getajob-0.7.0/getajob/test_support/fixtures/users.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/utils.py` & `getajob-0.7.0/getajob/utils.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/algolia/mock.py` & `getajob-0.7.0/getajob/vendor/algolia/mock.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/algolia/models.py` & `getajob-0.7.0/getajob/vendor/algolia/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/algolia/repository.py` & `getajob-0.7.0/getajob/vendor/algolia/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/clerk/client.py` & `getajob-0.7.0/getajob/vendor/clerk/client.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/clerk/companies/models.py` & `getajob-0.7.0/getajob/vendor/clerk/companies/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/clerk/companies/repository.py` & `getajob-0.7.0/getajob/vendor/clerk/companies/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/clerk/companies/unit_of_work.py` & `getajob-0.7.0/getajob/vendor/clerk/companies/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/clerk/mock.py` & `getajob-0.7.0/getajob/vendor/clerk/mock.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/clerk/recruiter_invitation/models.py` & `getajob-0.7.0/getajob/vendor/clerk/recruiter_invitation/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/clerk/recruiter_invitation/repository.py` & `getajob-0.7.0/getajob/vendor/clerk/recruiter_invitation/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/clerk/recruiters/models.py` & `getajob-0.7.0/getajob/vendor/clerk/recruiters/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/clerk/recruiters/repository.py` & `getajob-0.7.0/getajob/vendor/clerk/recruiters/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/clerk/repository.py` & `getajob-0.7.0/getajob/vendor/clerk/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/clerk/users/models.py` & `getajob-0.7.0/getajob/vendor/clerk/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/clerk/users/repository.py` & `getajob-0.7.0/getajob/vendor/clerk/users/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/firebase_storage/client_factory.py` & `getajob-0.7.0/getajob/vendor/firebase_storage/client_factory.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/firebase_storage/mock.py` & `getajob-0.7.0/getajob/vendor/firebase_storage/mock.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/firebase_storage/repository.py` & `getajob-0.7.0/getajob/vendor/firebase_storage/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/firestore/client_factory.py` & `getajob-0.7.0/getajob/vendor/firestore/client_factory.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/firestore/helpers.py` & `getajob-0.7.0/getajob/vendor/firestore/helpers.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/firestore/models.py` & `getajob-0.7.0/getajob/vendor/firestore/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/firestore/repository.py` & `getajob-0.7.0/getajob/vendor/firestore/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/jwt.py` & `getajob-0.7.0/getajob/vendor/jwt.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/kafka/client_factory.py` & `getajob-0.7.0/getajob/vendor/kafka/client_factory.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/kafka/mock.py` & `getajob-0.7.0/getajob/vendor/kafka/mock.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/kafka/models.py` & `getajob-0.7.0/getajob/vendor/kafka/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import Any, Type, Callable
+from typing import Any, Type, Callable, Union, Dict
 from enum import Enum
 from datetime import datetime
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 
 class KafkaGroup(str, Enum):
     DATA_SERVICES = "data_services"
     NOTIFICATION_SERVICES = "notification_services"
 
 
@@ -18,14 +18,16 @@
     """Audit is not needed, it is assumed for all messages"""
 
     users = "users"
     jobs = "jobs"
     companies = "companies"
     applications = "applications"
     chat = "chat"
+    api_logs = "api_logs"
+    search_logs = "search_logs"
 
     @classmethod
     def get_all_topics(cls):
         return [topic.value for topic in cls.__members__.values()]
 
 
 class KafkaEventConfig(BaseModel):
@@ -45,14 +47,42 @@
     requesting_user_id: str
     parent_collections: dict[str, str] = {}
     message_type: str  # This is any of the enum values below, handled by consumer
     message_time: datetime = datetime.now()
     data: dict[str, Any] | None = None
 
 
+class APILogMessage(BaseModel):
+    status_code: int
+    process_time: float
+    company_id: str | None
+    user_id: Union[str, int] = Field(default="anonymous")
+    user_email: str = Field(default="anonymous")
+    client_host: str = Field(default="unknown")
+    method: str
+    url: str
+    query_params: Dict[str, Any]
+    path_params: Dict[str, Any]
+    message_time: datetime = datetime.now()
+
+
+class SearchImpressionData(BaseModel):
+    index: str
+    hits: list[str]  # The ids of the hits
+    nbHits: int
+    page: int
+    query: str
+    params: str
+    search_time: datetime = datetime.now()
+
+
+class KafkaAPILogsEnum(str, Enum):
+    log = "log"
+
+
 class KafkaUsersEnum(str, Enum):
     create = "create_user"
     update = "update_user"
     delete = "delete_user"
 
 
 class KafkaUsersDetailsEnum(str, Enum):
@@ -64,15 +94,14 @@
     update = "update_user_resume_extraction"
 
 
 class KafkaJobsEnum(str, Enum):
     create = "create_job"
     update = "update_job"
     delete = "delete_job"
-    get = "get_job"
 
 
 class KafkaApplicationsEnum(str, Enum):
     create = "create_application"
     update = "update_application"
     delete = "delete_application"
 
@@ -90,15 +119,14 @@
 class KafkaCompanyDetailsEnum(str, Enum):
     update = "update_company_details"
 
 
 class KafkaCandidatesEnum(str, Enum):
     create = "create_candidate"
     update = "update_candidate"
-    get = "get_candidate"
 
 
 class KafkaChatEnum(str, Enum):
     create = "user_create_chat_message"
 
 
 class KafkaAuditEnum(str, Enum):
```

### Comparing `getajob-0.6.8/getajob/vendor/mailgun/client_factory.py` & `getajob-0.7.0/getajob/vendor/mailgun/client_factory.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/mailgun/repository.py` & `getajob-0.7.0/getajob/vendor/mailgun/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/openai/mock.py` & `getajob-0.7.0/getajob/vendor/openai/mock.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/openai/repository.py` & `getajob-0.7.0/getajob/vendor/openai/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/openai/settings.py` & `getajob-0.7.0/getajob/vendor/openai/settings.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/qstash/client.py` & `getajob-0.7.0/getajob/vendor/qstash/client.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/qstash/repository.py` & `getajob-0.7.0/getajob/vendor/qstash/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/getajob/vendor/redis/repository.py` & `getajob-0.7.0/getajob/vendor/redis/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.6.8/pyproject.toml` & `getajob-0.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getajob"
-version = "0.6.8"
+version = "0.7.0"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "3.8.4"
```

### Comparing `getajob-0.6.8/PKG-INFO` & `getajob-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getajob
-Version: 0.6.8
+Version: 0.7.0
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiocron (>=1.8,<2.0)
```

