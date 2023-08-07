# Comparing `tmp/leprikon-3.5.3.tar.gz` & `tmp/leprikon-3.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leprikon-3.5.3.tar", max compression
+gzip compressed data, was "leprikon-3.5.4.tar", max compression
```

## Comparing `leprikon-3.5.3.tar` & `leprikon-3.5.4.tar`

### file list

```diff
@@ -1,428 +1,428 @@
--rw-r--r--   0        0        0     1483 2021-02-06 20:07:27.966856 leprikon-3.5.3/LICENSE
--rw-r--r--   0        0        0      698 2021-02-06 20:07:27.966856 leprikon-3.5.3/README.rst
--rw-r--r--   0        0        0     6359 2023-08-07 14:40:02.485342 leprikon-3.5.3/leprikon/__init__.py
--rwxr-xr-x   0        0        0      326 2021-02-06 20:20:39.165125 leprikon-3.5.3/leprikon/__main__.py
--rw-r--r--   0        0        0     2366 2022-09-11 22:24:07.292086 leprikon-3.5.3/leprikon/admin/__init__.py
--rw-r--r--   0        0        0      194 2021-02-06 20:20:39.169125 leprikon-3.5.3/leprikon/admin/account.py
--rw-r--r--   0        0        0      341 2023-07-13 19:03:27.661576 leprikon-3.5.3/leprikon/admin/agegroup.py
--rw-r--r--   0        0        0     1215 2023-07-13 19:03:27.661576 leprikon-3.5.3/leprikon/admin/agreements.py
--rw-r--r--   0        0        0     3866 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/admin/bulkupdate.py
--rw-r--r--   0        0        0      316 2023-07-13 19:03:27.665576 leprikon-3.5.3/leprikon/admin/citizenship.py
--rw-r--r--   0        0        0    13805 2023-08-07 14:39:39.929427 leprikon-3.5.3/leprikon/admin/courses.py
--rw-r--r--   0        0        0      184 2021-02-06 20:20:39.169125 leprikon-3.5.3/leprikon/admin/department.py
--rw-r--r--   0        0        0     1280 2021-06-01 08:37:09.562968 leprikon-3.5.3/leprikon/admin/donation.py
--rw-r--r--   0        0        0     8853 2023-08-07 14:39:39.929427 leprikon-3.5.3/leprikon/admin/events.py
--rw-r--r--   0        0        0     4695 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/admin/export.py
--rw-r--r--   0        0        0     8990 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/admin/filters.py
--rw-r--r--   0        0        0     9088 2023-01-09 01:29:06.992459 leprikon-3.5.3/leprikon/admin/journals.py
--rw-r--r--   0        0        0      899 2023-01-20 02:25:46.109478 leprikon-3.5.3/leprikon/admin/leprikonsite.py
--rw-r--r--   0        0        0     8213 2023-01-09 01:29:06.992459 leprikon-3.5.3/leprikon/admin/messages.py
--rw-r--r--   0        0        0    10131 2023-08-07 14:39:39.929427 leprikon-3.5.3/leprikon/admin/orderables.py
--rw-r--r--   0        0        0      259 2021-02-06 20:20:39.173125 leprikon-3.5.3/leprikon/admin/organizations.py
--rw-r--r--   0        0        0     2469 2023-07-13 19:03:27.665576 leprikon-3.5.3/leprikon/admin/pdf.py
--rw-r--r--   0        0        0      165 2021-02-06 20:20:39.173125 leprikon-3.5.3/leprikon/admin/place.py
--rw-r--r--   0        0        0      190 2021-02-06 20:20:39.173125 leprikon-3.5.3/leprikon/admin/printsetup.py
--rw-r--r--   0        0        0      311 2022-06-19 21:02:37.423258 leprikon-3.5.3/leprikon/admin/question.py
--rw-r--r--   0        0        0     6405 2023-01-11 22:05:01.465080 leprikon-3.5.3/leprikon/admin/refundrequest.py
--rw-r--r--   0        0        0     5217 2023-07-30 15:02:55.324965 leprikon-3.5.3/leprikon/admin/registrationlink.py
--rw-r--r--   0        0        0     6294 2023-07-13 19:03:27.665576 leprikon-3.5.3/leprikon/admin/roles.py
--rw-r--r--   0        0        0      171 2021-02-06 20:20:39.173125 leprikon-3.5.3/leprikon/admin/school.py
--rw-r--r--   0        0        0     3454 2023-07-13 19:03:27.665576 leprikon-3.5.3/leprikon/admin/schoolyear.py
--rw-r--r--   0        0        0      399 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/admin/sendmail.py
--rw-r--r--   0        0        0    45734 2023-07-30 15:02:55.328965 leprikon-3.5.3/leprikon/admin/subjects.py
--rw-r--r--   0        0        0      310 2023-07-13 19:03:27.665576 leprikon-3.5.3/leprikon/admin/targetgroup.py
--rw-r--r--   0        0        0     4612 2023-07-13 19:26:09.899255 leprikon-3.5.3/leprikon/admin/timesheets.py
--rw-r--r--   0        0        0     7470 2023-01-10 14:07:38.306536 leprikon-3.5.3/leprikon/admin/transaction.py
--rw-r--r--   0        0        0     6951 2023-01-09 01:29:06.996459 leprikon-3.5.3/leprikon/admin/user.py
--rw-r--r--   0        0        0      635 2022-06-19 21:02:37.423258 leprikon-3.5.3/leprikon/admin/utils.py
--rw-r--r--   0        0        0        0 2021-02-06 20:07:27.974856 leprikon-3.5.3/leprikon/api/__init__.py
--rw-r--r--   0        0        0      165 2023-07-13 19:26:09.899255 leprikon-3.5.3/leprikon/api/openapi.py
--rw-r--r--   0        0        0      948 2023-04-17 11:27:57.487276 leprikon-3.5.3/leprikon/api/serializers.py
--rw-r--r--   0        0        0      778 2023-07-13 19:26:09.899255 leprikon-3.5.3/leprikon/api/urls.py
--rw-r--r--   0        0        0     3857 2023-07-30 15:02:55.328965 leprikon-3.5.3/leprikon/api/views.py
--rw-r--r--   0        0        0     1231 2023-04-17 11:27:57.487276 leprikon-3.5.3/leprikon/apps.py
--rw-r--r--   0        0        0     1091 2021-02-06 20:20:39.177125 leprikon-3.5.3/leprikon/bankreaders.py
--rw-r--r--   0        0        0     1263 2023-07-30 15:02:55.328965 leprikon-3.5.3/leprikon/cms_apps.py
--rw-r--r--   0        0        0     9366 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/cms_menus.py
--rw-r--r--   0        0        0      150 2021-02-06 20:07:27.978855 leprikon-3.5.3/leprikon/cms_plugins/__init__.py
--rw-r--r--   0        0        0      440 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/cms_plugins/base.py
--rw-r--r--   0        0        0     1097 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/cms_plugins/courses.py
--rw-r--r--   0        0        0     1080 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/cms_plugins/events.py
--rw-r--r--   0        0        0     1018 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/cms_plugins/leaders.py
--rw-r--r--   0        0        0     1154 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/cms_plugins/orderables.py
--rw-r--r--   0        0        0      466 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/cms_plugins/schoolyears.py
--rw-r--r--   0        0        0      683 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/cms_toolbars.py
--rw-r--r--   0        0        0      485 2021-02-06 20:20:39.181125 leprikon-3.5.3/leprikon/conf/__init__.py
--rw-r--r--   0        0        0     4015 2023-01-23 01:36:04.150478 leprikon-3.5.3/leprikon/conf/default_settings.py
--rw-r--r--   0        0        0     2234 2021-02-06 20:20:39.181125 leprikon-3.5.3/leprikon/cronjobs.py
--rw-r--r--   0        0        0        0 2021-02-06 20:07:27.982856 leprikon-3.5.3/leprikon/forms/__init__.py
--rw-r--r--   0        0        0      341 2021-02-06 20:20:39.181125 leprikon-3.5.3/leprikon/forms/billing_info.py
--rw-r--r--   0        0        0      319 2021-02-15 21:00:52.270425 leprikon-3.5.3/leprikon/forms/confirm.py
--rw-r--r--   0        0        0     2860 2023-08-01 20:24:04.264870 leprikon-3.5.3/leprikon/forms/courses.py
--rw-r--r--   0        0        0     2846 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/forms/fields.py
--rw-r--r--   0        0        0      610 2021-02-15 21:00:52.270425 leprikon-3.5.3/leprikon/forms/form.py
--rw-r--r--   0        0        0    18999 2023-07-30 15:02:55.328965 leprikon-3.5.3/leprikon/forms/journals.py
--rw-r--r--   0        0        0      780 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/forms/leaders.py
--rw-r--r--   0        0        0     2232 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/forms/messages.py
--rw-r--r--   0        0        0      326 2021-02-06 20:20:39.185125 leprikon-3.5.3/leprikon/forms/parent.py
--rw-r--r--   0        0        0      716 2021-02-06 20:20:39.185125 leprikon-3.5.3/leprikon/forms/participant.py
--rw-r--r--   0        0        0     3827 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/forms/refundrequest.py
--rw-r--r--   0        0        0      446 2022-06-19 21:02:37.423258 leprikon-3.5.3/leprikon/forms/registrationlink.py
--rw-r--r--   0        0        0        0 2021-02-06 20:07:28.054856 leprikon-3.5.3/leprikon/forms/reports/__init__.py
--rw-r--r--   0        0        0     1477 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/forms/reports/courses.py
--rw-r--r--   0        0        0      209 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/forms/reports/debtors.py
--rw-r--r--   0        0        0     1463 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/forms/reports/events.py
--rw-r--r--   0        0        0     1503 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/forms/reports/orderables.py
--rw-r--r--   0        0        0      715 2022-09-11 22:24:07.296086 leprikon-3.5.3/leprikon/forms/schoolyear.py
--rw-r--r--   0        0        0    39013 2023-08-01 20:10:29.970532 leprikon-3.5.3/leprikon/forms/subjects.py
--rw-r--r--   0        0        0     3521 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/forms/timesheets.py
--rw-r--r--   0        0        0     4245 2023-04-17 11:27:57.487276 leprikon-3.5.3/leprikon/forms/user.py
--rw-r--r--   0        0        0     1088 2022-06-19 21:02:37.427258 leprikon-3.5.3/leprikon/forms/widgets.py
--rw-r--r--   0        0        0      209 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/gettext_overrides.py
--rw-r--r--   0        0        0    77353 2023-08-01 20:22:30.958943 leprikon-3.5.3/leprikon/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   141305 2023-08-01 20:22:38.343558 leprikon-3.5.3/leprikon/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      323 2022-09-04 23:40:36.644492 leprikon-3.5.3/leprikon/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   111732 2022-09-04 22:12:01.810032 leprikon-3.5.3/leprikon/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2021-02-06 20:07:28.070855 leprikon-3.5.3/leprikon/management/__init__.py
--rw-r--r--   0        0        0        0 2021-02-06 20:07:28.070855 leprikon-3.5.3/leprikon/management/commands/__init__.py
--rw-r--r--   0        0        0     4121 2022-06-19 21:02:37.431258 leprikon-3.5.3/leprikon/middleware.py
--rw-r--r--   0        0        0    59583 2023-01-23 01:36:04.150478 leprikon-3.5.3/leprikon/migrations/0001_initial.py
--rw-r--r--   0        0        0     1851 2021-02-06 20:07:28.070855 leprikon-3.5.3/leprikon/migrations/0002_initial_data.py
--rw-r--r--   0        0        0     1954 2021-02-06 20:07:28.070855 leprikon-3.5.3/leprikon/migrations/0003_managers.py
--rw-r--r--   0        0        0      345 2021-02-06 20:07:28.070855 leprikon-3.5.3/leprikon/migrations/0004_multiple_registrations.py
--rw-r--r--   0        0        0      879 2021-02-06 20:07:28.070855 leprikon-3.5.3/leprikon/migrations/0005_subjectregistration_variable_symbol.py
--rw-r--r--   0        0        0     1049 2021-02-06 20:07:28.070855 leprikon-3.5.3/leprikon/migrations/0006_discount_periods.py
--rw-r--r--   0        0        0      864 2021-02-06 20:07:28.070855 leprikon-3.5.3/leprikon/migrations/0007_bill_print_setup.py
--rw-r--r--   0        0        0      449 2021-02-06 20:07:28.070855 leprikon-3.5.3/leprikon/migrations/0008_leprikonsite_company_name.py
--rw-r--r--   0        0        0      656 2021-02-06 20:07:28.070855 leprikon-3.5.3/leprikon/migrations/0009_subjectpayment_received_by.py
--rw-r--r--   0        0        0      449 2021-02-06 20:07:28.070855 leprikon-3.5.3/leprikon/migrations/0010_subject_code.py
--rw-r--r--   0        0        0      457 2021-02-06 20:07:28.070855 leprikon-3.5.3/leprikon/migrations/0011_subjectregistration_payment_requested.py
--rw-r--r--   0        0        0     1720 2023-08-01 20:22:11.113519 leprikon-3.5.3/leprikon/migrations/0012_subject_variants.py
--rw-r--r--   0        0        0      549 2021-02-06 20:07:28.070855 leprikon-3.5.3/leprikon/migrations/0013_drop_insurance.py
--rw-r--r--   0        0        0      472 2021-02-06 20:07:28.070855 leprikon-3.5.3/leprikon/migrations/0014_variable_symbol.py
--rw-r--r--   0        0        0     4137 2021-02-06 20:07:28.070855 leprikon-3.5.3/leprikon/migrations/0015_school_year_divisions.py
--rw-r--r--   0        0        0     1191 2021-02-06 20:07:28.070855 leprikon-3.5.3/leprikon/migrations/0016_school_year_divisions_cleanup.py
--rw-r--r--   0        0        0     3919 2023-07-13 19:03:27.669576 leprikon-3.5.3/leprikon/migrations/0017_citizenship.py
--rw-r--r--   0        0        0      475 2021-02-06 20:07:28.070855 leprikon-3.5.3/leprikon/migrations/0018_citizenship_cleanup.py
--rw-r--r--   0        0        0     3040 2021-02-06 20:07:28.070855 leprikon-3.5.3/leprikon/migrations/0019_department.py
--rw-r--r--   0        0        0     1377 2021-02-06 20:07:28.070855 leprikon-3.5.3/leprikon/migrations/0020_agreements.py
--rw-r--r--   0        0        0     1532 2021-02-06 20:07:28.074856 leprikon-3.5.3/leprikon/migrations/0021_user_agreement.py
--rw-r--r--   0        0        0      671 2021-02-06 20:07:28.074856 leprikon-3.5.3/leprikon/migrations/0022_bankreader.py
--rw-r--r--   0        0        0     2506 2021-02-06 20:07:28.074856 leprikon-3.5.3/leprikon/migrations/0023_accountclosure.py
--rw-r--r--   0        0        0      504 2021-02-06 20:07:28.074856 leprikon-3.5.3/leprikon/migrations/0024_subjectregistration_note.py
--rw-r--r--   0        0        0     5224 2021-02-06 20:07:28.074856 leprikon-3.5.3/leprikon/migrations/0025_agreements.py
--rw-r--r--   0        0        0      942 2021-02-06 20:07:28.074856 leprikon-3.5.3/leprikon/migrations/0026_online_payments.py
--rw-r--r--   0        0        0     2243 2021-02-06 20:07:28.074856 leprikon-3.5.3/leprikon/migrations/0027_journals.py
--rw-r--r--   0        0        0      517 2021-02-06 20:07:28.074856 leprikon-3.5.3/leprikon/migrations/0028_agegroups.py
--rw-r--r--   0        0        0      646 2021-02-06 20:07:28.074856 leprikon-3.5.3/leprikon/migrations/0029_payment_restrictions.py
--rw-r--r--   0        0        0      716 2021-02-06 20:07:28.074856 leprikon-3.5.3/leprikon/migrations/0030_agreements.py
--rw-r--r--   0        0        0     2208 2021-02-06 20:07:28.074856 leprikon-3.5.3/leprikon/migrations/0031_registration_questions_agreements.py
--rw-r--r--   0        0        0    15532 2021-02-06 20:07:28.074856 leprikon-3.5.3/leprikon/migrations/0032_registration_participants_groups.py
--rw-r--r--   0        0        0     4196 2021-02-06 20:07:28.074856 leprikon-3.5.3/leprikon/migrations/0033_target_groups.py
--rw-r--r--   0        0        0     9741 2022-09-11 14:45:14.421101 leprikon-3.5.3/leprikon/migrations/0034_subject_registration_group.py
--rw-r--r--   0        0        0     1807 2021-02-06 20:07:28.078856 leprikon-3.5.3/leprikon/migrations/0035_on_delete.py
--rw-r--r--   0        0        0     1220 2021-02-06 20:07:28.078856 leprikon-3.5.3/leprikon/migrations/0036_participants_instructed.py
--rw-r--r--   0        0        0      703 2021-02-06 20:07:28.078856 leprikon-3.5.3/leprikon/migrations/0037_message_sender.py
--rw-r--r--   0        0        0     6559 2021-02-06 20:07:28.078856 leprikon-3.5.3/leprikon/migrations/0038_organizations.py
--rw-r--r--   0        0        0     4941 2021-02-06 20:07:28.078856 leprikon-3.5.3/leprikon/migrations/0039_editable_texts.py
--rw-r--r--   0        0        0     1827 2021-02-06 20:07:28.078856 leprikon-3.5.3/leprikon/migrations/0040_due_dates.py
--rw-r--r--   0        0        0     2946 2021-02-06 20:07:28.082856 leprikon-3.5.3/leprikon/migrations/0041_billing_info.py
--rw-r--r--   0        0        0     1207 2021-02-06 20:07:28.082856 leprikon-3.5.3/leprikon/migrations/0042_chat_group_types.py
--rw-r--r--   0        0        0     1960 2021-02-06 20:07:28.082856 leprikon-3.5.3/leprikon/migrations/0043_registration_links.py
--rw-r--r--   0        0        0     2153 2021-02-06 20:07:28.082856 leprikon-3.5.3/leprikon/migrations/0044_billinginfo_contacts.py
--rw-r--r--   0        0        0      527 2021-02-06 20:07:28.082856 leprikon-3.5.3/leprikon/migrations/0045_registration_slug.py
--rw-r--r--   0        0        0     3632 2021-02-06 20:07:28.082856 leprikon-3.5.3/leprikon/migrations/0046_attachment_events.py
--rw-r--r--   0        0        0     6061 2021-02-06 20:07:28.086856 leprikon-3.5.3/leprikon/migrations/0047_pr_print_setup.py
--rw-r--r--   0        0        0     2700 2021-02-06 20:07:28.086856 leprikon-3.5.3/leprikon/migrations/0048_birth_date.py
--rw-r--r--   0        0        0      999 2021-02-06 20:07:28.086856 leprikon-3.5.3/leprikon/migrations/0049_target_groups_fix.py
--rw-r--r--   0        0        0    11512 2022-06-19 21:02:37.431258 leprikon-3.5.3/leprikon/migrations/0050_orderables.py
--rw-r--r--   0        0        0      546 2021-02-06 20:07:28.086856 leprikon-3.5.3/leprikon/migrations/0051_registration_group_name.py
--rw-r--r--   0        0        0      762 2021-02-06 20:07:28.086856 leprikon-3.5.3/leprikon/migrations/0052_payment_notification_sent.py
--rw-r--r--   0        0        0     2528 2021-02-06 20:07:28.090856 leprikon-3.5.3/leprikon/migrations/0053_registration_dates_by.py
--rw-r--r--   0        0        0      460 2021-02-06 20:07:28.090856 leprikon-3.5.3/leprikon/migrations/0054_registration_dates_by_cleanup.py
--rw-r--r--   0        0        0     1020 2021-02-06 20:07:28.090856 leprikon-3.5.3/leprikon/migrations/0055_schoolyearblockplugin.py
--rw-r--r--   0        0        0     4108 2021-02-06 20:07:28.090856 leprikon-3.5.3/leprikon/migrations/0056_registration_period.py
--rw-r--r--   0        0        0      739 2021-02-06 20:07:28.094856 leprikon-3.5.3/leprikon/migrations/0057_registration_period.py
--rw-r--r--   0        0        0     1229 2021-02-06 20:07:28.094856 leprikon-3.5.3/leprikon/migrations/0058_agegroup_min_max_age.py
--rw-r--r--   0        0        0     5253 2021-07-30 12:23:56.621387 leprikon-3.5.3/leprikon/migrations/0059_transactions_data.py
--rw-r--r--   0        0        0    12344 2021-06-03 01:45:58.168248 leprikon-3.5.3/leprikon/migrations/0060_transactions.py
--rw-r--r--   0        0        0     2055 2021-06-03 02:51:13.941010 leprikon-3.5.3/leprikon/migrations/0061_refundrequest.py
--rw-r--r--   0        0        0     4102 2021-06-08 21:18:56.417557 leprikon-3.5.3/leprikon/migrations/0062_refund_offers.py
--rw-r--r--   0        0        0     7724 2021-08-31 21:32:49.271400 leprikon-3.5.3/leprikon/migrations/0063_journals.py
--rw-r--r--   0        0        0     1127 2021-10-26 23:31:48.142344 leprikon-3.5.3/leprikon/migrations/0064_journals_cleanup.py
--rw-r--r--   0        0        0     1600 2022-06-19 21:02:37.431258 leprikon-3.5.3/leprikon/migrations/0065_subject_type_page.py
--rw-r--r--   0        0        0      453 2022-06-19 21:02:37.431258 leprikon-3.5.3/leprikon/migrations/0066_subject_type_slug_unique.py
--rw-r--r--   0        0        0      528 2022-06-19 21:02:37.431258 leprikon-3.5.3/leprikon/migrations/0067_remove_rocketchat.py
--rw-r--r--   0        0        0      518 2022-06-19 21:02:37.431258 leprikon-3.5.3/leprikon/migrations/0068_participant_answers.py
--rw-r--r--   0        0        0     2329 2023-01-20 01:19:05.975668 leprikon-3.5.3/leprikon/migrations/0069_question_slug.py
--rw-r--r--   0        0        0     1851 2023-01-20 01:19:05.975668 leprikon-3.5.3/leprikon/migrations/0070_decision_print_setup.py
--rw-r--r--   0        0        0      746 2022-09-04 23:40:36.644492 leprikon-3.5.3/leprikon/migrations/0071_transaction_amount.py
--rw-r--r--   0        0        0     9100 2022-09-11 15:35:00.764956 leprikon-3.5.3/leprikon/migrations/0072_prices.py
--rw-r--r--   0        0        0     3555 2023-01-23 01:36:04.150478 leprikon-3.5.3/leprikon/migrations/0073_add_limit_choices_to.py
--rw-r--r--   0        0        0     1311 2023-01-09 01:29:06.996459 leprikon-3.5.3/leprikon/migrations/0074_schoolyear_period_order.py
--rw-r--r--   0        0        0     3311 2023-07-30 15:02:55.328965 leprikon-3.5.3/leprikon/migrations/0075_journal_school_year_division.py
--rw-r--r--   0        0        0     1603 2023-01-09 01:29:06.996459 leprikon-3.5.3/leprikon/migrations/0076_journalentry_period.py
--rw-r--r--   0        0        0      482 2023-01-23 01:36:04.150478 leprikon-3.5.3/leprikon/migrations/0077_place_description.py
--rw-r--r--   0        0        0     1840 2023-07-13 19:03:27.669576 leprikon-3.5.3/leprikon/migrations/0078_delete_coursevariant.py
--rw-r--r--   0        0        0     8301 2023-08-01 20:10:29.970532 leprikon-3.5.3/leprikon/migrations/0079_mandatory_subject_variants.py
--rw-r--r--   0        0        0        0 2021-02-06 20:07:28.094856 leprikon-3.5.3/leprikon/migrations/__init__.py
--rw-r--r--   0        0        0      463 2021-06-03 02:51:13.941010 leprikon-3.5.3/leprikon/models/__init__.py
--rw-r--r--   0        0        0      641 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/models/account.py
--rw-r--r--   0        0        0      793 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/models/agegroup.py
--rw-r--r--   0        0        0     1553 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/models/agreements.py
--rw-r--r--   0        0        0      540 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/models/citizenship.py
--rw-r--r--   0        0        0    17737 2023-07-30 15:02:55.332965 leprikon-3.5.3/leprikon/models/courses.py
--rw-r--r--   0        0        0      616 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/models/department.py
--rw-r--r--   0        0        0      704 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/models/donation.py
--rw-r--r--   0        0        0    12356 2023-07-30 15:02:55.332965 leprikon-3.5.3/leprikon/models/events.py
--rw-r--r--   0        0        0     5763 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/models/fields.py
--rw-r--r--   0        0        0    10471 2023-07-30 15:02:55.332965 leprikon-3.5.3/leprikon/models/journals.py
--rw-r--r--   0        0        0     3367 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/models/leprikonsite.py
--rw-r--r--   0        0        0     4316 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/models/messages.py
--rw-r--r--   0        0        0    12852 2023-07-30 15:02:55.332965 leprikon-3.5.3/leprikon/models/orderables.py
--rw-r--r--   0        0        0     1896 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/models/organizations.py
--rw-r--r--   0        0        0     4129 2023-07-13 19:03:27.669576 leprikon-3.5.3/leprikon/models/pdfmail.py
--rw-r--r--   0        0        0      714 2023-01-23 01:36:04.150478 leprikon-3.5.3/leprikon/models/place.py
--rw-r--r--   0        0        0     2183 2023-07-13 19:03:27.669576 leprikon-3.5.3/leprikon/models/printsetup.py
--rw-r--r--   0        0        0     2093 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/models/question.py
--rw-r--r--   0        0        0     1625 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/models/refundrequest.py
--rw-r--r--   0        0        0     1730 2023-07-30 15:02:55.332965 leprikon-3.5.3/leprikon/models/registrationlink.py
--rw-r--r--   0        0        0    12114 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/models/roles.py
--rw-r--r--   0        0        0      894 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/models/school.py
--rw-r--r--   0        0        0     5005 2023-01-09 01:29:06.996459 leprikon-3.5.3/leprikon/models/schoolyear.py
--rw-r--r--   0        0        0      639 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/models/startend.py
--rw-r--r--   0        0        0    68416 2023-08-01 20:13:53.729874 leprikon-3.5.3/leprikon/models/subjects.py
--rw-r--r--   0        0        0      626 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/models/targetgroup.py
--rw-r--r--   0        0        0     1482 2021-06-03 03:12:18.850194 leprikon-3.5.3/leprikon/models/test_utils.py
--rw-r--r--   0        0        0     2787 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/models/times.py
--rw-r--r--   0        0        0     5592 2023-01-20 01:19:05.979668 leprikon-3.5.3/leprikon/models/timesheets.py
--rw-r--r--   0        0        0     9259 2023-01-20 01:19:05.979668 leprikon-3.5.3/leprikon/models/transaction.py
--rw-r--r--   0        0        0      439 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/models/useragreement.py
--rw-r--r--   0        0        0     9133 2023-07-30 15:02:55.336964 leprikon-3.5.3/leprikon/models/utils.py
--rw-r--r--   0        0        0      127 2021-02-06 20:07:28.098856 leprikon-3.5.3/leprikon/search_indexes/__init__.py
--rw-r--r--   0        0        0      682 2021-02-06 20:20:39.189125 leprikon-3.5.3/leprikon/search_indexes/base.py
--rw-r--r--   0        0        0      143 2021-02-06 20:20:39.189125 leprikon-3.5.3/leprikon/search_indexes/courses.py
--rw-r--r--   0        0        0      139 2021-02-06 20:20:39.189125 leprikon-3.5.3/leprikon/search_indexes/events.py
--rw-r--r--   0        0        0      155 2021-02-06 20:20:39.189125 leprikon-3.5.3/leprikon/search_indexes/orderables.py
--rw-r--r--   0        0        0        0 2021-02-06 20:07:28.102856 leprikon-3.5.3/leprikon/site/__init__.py
--rw-r--r--   0        0        0    16830 2023-07-30 15:02:55.336964 leprikon-3.5.3/leprikon/site/settings.py
--rw-r--r--   0        0        0     1761 2023-07-17 19:51:19.009803 leprikon-3.5.3/leprikon/site/urls.py
--rw-r--r--   0        0        0      458 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/site/wsgi.py
--rw-r--r--   0        0        0      566 2023-01-20 01:19:05.979668 leprikon-3.5.3/leprikon/static/admin/css/scrollbars.css
--rw-r--r--   0        0        0     5994 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/static/admin/js/admin/RelatedObjectLookups.js
--rw-r--r--   0        0        0    10366 2021-02-06 20:07:28.102856 leprikon-3.5.3/leprikon/static/favicon.ico
--rw-r--r--   0        0        0     3153 2021-02-06 20:07:28.102856 leprikon-3.5.3/leprikon/static/leprikon/css/colors.css
--rw-r--r--   0        0        0     4472 2021-02-06 20:07:28.102856 leprikon-3.5.3/leprikon/static/leprikon/css/layout.css
--rw-r--r--   0        0        0     1138 2021-02-06 20:07:28.102856 leprikon-3.5.3/leprikon/static/leprikon/css/registrations.changelist.css
--rw-r--r--   0        0        0   705684 2021-02-06 20:07:28.118856 leprikon-3.5.3/leprikon/static/leprikon/fonts/DejaVuSans-Bold.ttf
--rw-r--r--   0        0        0   643292 2021-02-06 20:07:28.126856 leprikon-3.5.3/leprikon/static/leprikon/fonts/DejaVuSans-BoldOblique.ttf
--rw-r--r--   0        0        0   635416 2021-02-06 20:07:28.134856 leprikon-3.5.3/leprikon/static/leprikon/fonts/DejaVuSans-Oblique.ttf
--rw-r--r--   0        0        0   757076 2021-02-06 20:07:28.138856 leprikon-3.5.3/leprikon/static/leprikon/fonts/DejaVuSans.ttf
--rw-r--r--   0        0        0    83151 2021-02-06 20:07:28.138856 leprikon-3.5.3/leprikon/static/leprikon/img/leprikon-kuk-l.png
--rw-r--r--   0        0        0    51531 2021-02-06 20:07:28.138856 leprikon-3.5.3/leprikon/static/leprikon/img/logo-horizontal.png
--rw-r--r--   0        0        0   200727 2021-02-06 20:07:28.138856 leprikon-3.5.3/leprikon/static/leprikon/img/logo.png
--rw-r--r--   0        0        0      522 2021-02-06 20:07:28.138856 leprikon-3.5.3/leprikon/static/leprikon/js/Popup.js
--rw-r--r--   0        0        0     1517 2022-06-19 21:02:37.435258 leprikon-3.5.3/leprikon/static/leprikon/js/required_optional_field.js
--rw-r--r--   0        0        0      175 2023-01-09 01:29:07.000459 leprikon-3.5.3/leprikon/staticfiles.py
--rw-r--r--   0        0        0      727 2021-02-06 20:07:28.142856 leprikon-3.5.3/leprikon/templates/admin/base.html
--rw-r--r--   0        0        0     1175 2021-02-06 20:07:28.142856 leprikon-3.5.3/leprikon/templates/admin/change_list.html
--rw-r--r--   0        0        0     1570 2021-02-06 20:07:28.142856 leprikon-3.5.3/leprikon/templates/admin/change_list_results.html
--rw-r--r--   0        0        0     1589 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/templates/admin/inc/branding.html
--rw-r--r--   0        0        0       96 2021-02-06 20:07:28.142856 leprikon-3.5.3/leprikon/templates/admin/inc/extrahead.html
--rw-r--r--   0        0        0      134 2021-02-06 20:07:28.142856 leprikon-3.5.3/leprikon/templates/admin/leprikon/app_index.html
--rw-r--r--   0        0        0      207 2021-02-06 20:07:28.142856 leprikon-3.5.3/leprikon/templates/admin/leprikon/coursediscount/popup_response.html
--rw-r--r--   0        0        0      561 2021-06-01 05:03:47.670256 leprikon-3.5.3/leprikon/templates/admin/leprikon/donation/change_form.html
--rw-r--r--   0        0        0      207 2021-02-06 20:07:28.142856 leprikon-3.5.3/leprikon/templates/admin/leprikon/eventdiscount/popup_response.html
--rw-r--r--   0        0        0      563 2021-02-06 20:07:28.142856 leprikon-3.5.3/leprikon/templates/admin/leprikon/message/add_recipients.html
--rw-r--r--   0        0        0      460 2021-02-06 20:07:28.142856 leprikon-3.5.3/leprikon/templates/admin/leprikon/messagerecipient/change_list.html
--rw-r--r--   0        0        0     2425 2021-02-06 20:07:28.142856 leprikon-3.5.3/leprikon/templates/admin/leprikon/messagerecipient/send_mails.html
--rw-r--r--   0        0        0      207 2021-02-06 20:07:28.142856 leprikon-3.5.3/leprikon/templates/admin/leprikon/orderablediscount/popup_response.html
--rw-r--r--   0        0        0      560 2021-06-01 05:03:47.670256 leprikon-3.5.3/leprikon/templates/admin/leprikon/subjectreceivedpayment/change_form.html
--rw-r--r--   0        0        0      207 2021-06-01 05:03:47.670256 leprikon-3.5.3/leprikon/templates/admin/leprikon/subjectreceivedpayment/popup_response.html
--rw-r--r--   0        0        0      560 2021-06-01 05:03:47.670256 leprikon-3.5.3/leprikon/templates/admin/leprikon/subjectreturnedpayment/change_form.html
--rw-r--r--   0        0        0      207 2021-05-31 17:36:24.566151 leprikon-3.5.3/leprikon/templates/admin/leprikon/subjectreturnedpayment/popup_response.html
--rw-r--r--   0        0        0        0 2021-02-06 20:07:28.142856 leprikon-3.5.3/leprikon/templates/auth/widgets/read_only_password_hash.html
--rw-r--r--   0        0        0      257 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/templates/cms/toolbar/items/logo.html
--rw-r--r--   0        0        0     1180 2021-02-06 20:07:28.142856 leprikon-3.5.3/leprikon/templates/leprikon/admin/action_form.html
--rw-r--r--   0        0        0     1170 2023-01-09 01:29:07.000459 leprikon-3.5.3/leprikon/templates/leprikon/admin/bulk_update_form.html
--rw-r--r--   0        0        0     2978 2021-08-16 07:31:28.779948 leprikon-3.5.3/leprikon/templates/leprikon/admin/dashboard.html
--rw-r--r--   0        0        0     1235 2021-02-06 20:07:28.142856 leprikon-3.5.3/leprikon/templates/leprikon/admin/merge.html
--rw-r--r--   0        0        0     1077 2021-02-06 20:07:28.142856 leprikon-3.5.3/leprikon/templates/leprikon/admin/send_message.html
--rw-r--r--   0        0        0     1296 2021-02-06 20:07:28.142856 leprikon-3.5.3/leprikon/templates/leprikon/alternating.html
--rw-r--r--   0        0        0     3431 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/templates/leprikon/base.html
--rw-r--r--   0        0        0     1089 2021-02-06 20:07:28.142856 leprikon-3.5.3/leprikon/templates/leprikon/billing_info_preview.html
--rw-r--r--   0        0        0       73 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/cms/course/default.html
--rw-r--r--   0        0        0      142 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/cms/course_list/default.html
--rw-r--r--   0        0        0      326 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/cms/course_list/grouped.html
--rw-r--r--   0        0        0     1368 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/templates/leprikon/cms/course_list_filtered.html
--rw-r--r--   0        0        0       70 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/cms/event/default.html
--rw-r--r--   0        0        0      139 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/cms/event_list/default.html
--rw-r--r--   0        0        0      324 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/cms/event_list/grouped.html
--rw-r--r--   0        0        0     1001 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/templates/leprikon/cms/event_list_filtered.html
--rw-r--r--   0        0        0       73 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/cms/leader/default.html
--rw-r--r--   0        0        0     1695 2023-08-07 14:40:02.485342 leprikon-3.5.3/leprikon/templates/leprikon/cms/leader_list/default.html
--rw-r--r--   0        0        0     1086 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/templates/leprikon/cms/leader_list_filtered.html
--rw-r--r--   0        0        0       82 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/cms/orderable/default.html
--rw-r--r--   0        0        0      151 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/cms/orderable_list/default.html
--rw-r--r--   0        0        0      332 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/cms/orderable_list/grouped.html
--rw-r--r--   0        0        0     1013 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/templates/leprikon/cms/orderable_list_filtered.html
--rw-r--r--   0        0        0      206 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/cms/school_year_block.html
--rw-r--r--   0        0        0      199 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/cms.html
--rw-r--r--   0        0        0      769 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/confirm_form.html
--rw-r--r--   0        0        0      224 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/course_detail.html
--rw-r--r--   0        0        0       65 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/course_preview.html
--rw-r--r--   0        0        0     1198 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/course_registrations.html
--rw-r--r--   0        0        0       35 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/default.html
--rw-r--r--   0        0        0     2470 2021-06-01 02:09:02.932873 leprikon-3.5.3/leprikon/templates/leprikon/donation_pdf/default.rml
--rw-r--r--   0        0        0     2701 2021-06-01 05:24:24.368881 leprikon-3.5.3/leprikon/templates/leprikon/donation_pdf/recipe.rml
--rw-r--r--   0        0        0      937 2021-06-01 09:11:38.676158 leprikon-3.5.3/leprikon/templates/leprikon/donations.html
--rw-r--r--   0        0        0      223 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/event_detail.html
--rw-r--r--   0        0        0       64 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/event_preview.html
--rw-r--r--   0        0        0     1187 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/event_registrations.html
--rw-r--r--   0        0        0      732 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/filter_form.html
--rw-r--r--   0        0        0     1991 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/templates/leprikon/filtered_subject_list.html
--rw-r--r--   0        0        0     2198 2021-08-31 20:34:46.158520 leprikon-3.5.3/leprikon/templates/leprikon/form.html
--rw-r--r--   0        0        0      254 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/form_inline_item.html
--rw-r--r--   0        0        0      493 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/form_item.html
--rw-r--r--   0        0        0      604 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/form_item_checkbox.html
--rw-r--r--   0        0        0      368 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/form_item_fullwidth.html
--rw-r--r--   0        0        0     7105 2023-01-09 01:29:07.000459 leprikon-3.5.3/leprikon/templates/leprikon/invoices.xml
--rw-r--r--   0        0        0      531 2022-09-11 22:24:07.300086 leprikon-3.5.3/leprikon/templates/leprikon/journal_form.html
--rw-r--r--   0        0        0    12058 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/journal_journal.html
--rw-r--r--   0        0        0     2271 2021-08-16 07:31:28.779948 leprikon-3.5.3/leprikon/templates/leprikon/journal_journal_pdf/default.rml
--rw-r--r--   0        0        0     2023 2022-06-19 21:02:37.435258 leprikon-3.5.3/leprikon/templates/leprikon/journal_preview.html
--rw-r--r--   0        0        0     2481 2023-07-30 15:02:55.336964 leprikon-3.5.3/leprikon/templates/leprikon/journalentry_form.html
--rw-r--r--   0        0        0      189 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/journalleaderentry_form.html
--rw-r--r--   0        0        0     1006 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/leader_list.html
--rw-r--r--   0        0        0     2220 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/leader_preview.html
--rw-r--r--   0        0        0      553 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/leader_summary.html
--rw-r--r--   0        0        0      743 2021-02-06 20:07:28.146856 leprikon-3.5.3/leprikon/templates/leprikon/list.html
--rw-r--r--   0        0        0     4959 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/login.html
--rw-r--r--   0        0        0      543 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/menu.html
--rw-r--r--   0        0        0      222 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/message_list.html
--rw-r--r--   0        0        0      320 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/message_mail.html
--rw-r--r--   0        0        0      222 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/message_mail.txt
--rw-r--r--   0        0        0      735 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/messagerecipient_detail.html
--rw-r--r--   0        0        0      586 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/messages_table.html
--rw-r--r--   0        0        0     1021 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/modal_messages.html
--rw-r--r--   0        0        0      227 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/orderable_detail.html
--rw-r--r--   0        0        0       68 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/orderable_preview.html
--rw-r--r--   0        0        0     1231 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/orderable_registrations.html
--rw-r--r--   0        0        0      898 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/pagination.html
--rw-r--r--   0        0        0      915 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/parent_preview.html
--rw-r--r--   0        0        0     1742 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/participant_preview.html
--rw-r--r--   0        0        0      443 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/participants.html
--rw-r--r--   0        0        0       35 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/password.html
--rw-r--r--   0        0        0      222 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/password_change_done.html
--rw-r--r--   0        0        0       35 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/password_reset.html
--rw-r--r--   0        0        0      368 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/password_reset_complete.html
--rw-r--r--   0        0        0       35 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/password_reset_confirm.html
--rw-r--r--   0        0        0      439 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/password_reset_done.html
--rw-r--r--   0        0        0      592 2021-02-06 20:07:28.150856 leprikon-3.5.3/leprikon/templates/leprikon/password_reset_email.html
--rw-r--r--   0        0        0     1617 2021-06-01 22:52:10.045174 leprikon-3.5.3/leprikon/templates/leprikon/payments.html
--rw-r--r--   0        0        0     2936 2021-06-01 08:37:09.562968 leprikon-3.5.3/leprikon/templates/leprikon/received_payment_pdf/recipe.rml
--rw-r--r--   0        0        0     2486 2021-06-01 08:37:09.562968 leprikon-3.5.3/leprikon/templates/leprikon/received_payment_pdf/subject.rml
--rw-r--r--   0        0        0      136 2021-06-01 08:37:09.566968 leprikon-3.5.3/leprikon/templates/leprikon/received_payment_received/subject.html
--rw-r--r--   0        0        0      223 2021-06-01 08:37:09.566968 leprikon-3.5.3/leprikon/templates/leprikon/received_payment_received/subject.subject.txt
--rw-r--r--   0        0        0      145 2021-06-01 08:37:09.566968 leprikon-3.5.3/leprikon/templates/leprikon/received_payment_received/subject.txt
--rw-r--r--   0        0        0      153 2021-02-06 20:07:28.154856 leprikon-3.5.3/leprikon/templates/leprikon/registration_approved/subject.html
--rw-r--r--   0        0        0      178 2021-06-01 02:09:02.932873 leprikon-3.5.3/leprikon/templates/leprikon/registration_approved/subject.subject.txt
--rw-r--r--   0        0        0      161 2021-02-06 20:07:28.154856 leprikon-3.5.3/leprikon/templates/leprikon/registration_approved/subject.txt
--rw-r--r--   0        0        0      153 2021-02-06 20:07:28.154856 leprikon-3.5.3/leprikon/templates/leprikon/registration_canceled/subject.html
--rw-r--r--   0        0        0      178 2021-06-01 02:09:02.932873 leprikon-3.5.3/leprikon/templates/leprikon/registration_canceled/subject.subject.txt
--rw-r--r--   0        0        0      161 2021-02-06 20:07:28.154856 leprikon-3.5.3/leprikon/templates/leprikon/registration_canceled/subject.txt
--rw-r--r--   0        0        0     5431 2022-06-19 23:56:58.526604 leprikon-3.5.3/leprikon/templates/leprikon/registration_decision/subject.rml
--rw-r--r--   0        0        0     6268 2021-02-06 20:07:28.154856 leprikon-3.5.3/leprikon/templates/leprikon/registration_details.html
--rw-r--r--   0        0        0     1209 2022-08-09 07:23:11.034741 leprikon-3.5.3/leprikon/templates/leprikon/registration_links.html
--rw-r--r--   0        0        0      610 2021-06-08 20:34:42.425099 leprikon-3.5.3/leprikon/templates/leprikon/registration_mail_details.html
--rw-r--r--   0        0        0      534 2021-06-08 20:34:42.425099 leprikon-3.5.3/leprikon/templates/leprikon/registration_mail_details.txt
--rw-r--r--   0        0        0      300 2021-02-06 20:07:28.154856 leprikon-3.5.3/leprikon/templates/leprikon/registration_mail_footer.html
--rw-r--r--   0        0        0      189 2021-02-06 20:07:28.154856 leprikon-3.5.3/leprikon/templates/leprikon/registration_mail_footer.txt
--rw-r--r--   0        0        0      427 2021-08-16 07:31:28.779948 leprikon-3.5.3/leprikon/templates/leprikon/registration_participant_presence.html
--rw-r--r--   0        0        0     1568 2021-02-06 20:07:28.154856 leprikon-3.5.3/leprikon/templates/leprikon/registration_payment_request/subject.html
--rw-r--r--   0        0        0    12348 2021-02-06 20:07:28.154856 leprikon-3.5.3/leprikon/templates/leprikon/registration_payment_request/subject.rml
--rw-r--r--   0        0        0      183 2021-06-01 02:09:02.932873 leprikon-3.5.3/leprikon/templates/leprikon/registration_payment_request/subject.subject.txt
--rw-r--r--   0        0        0     1172 2021-02-06 20:07:28.154856 leprikon-3.5.3/leprikon/templates/leprikon/registration_payment_request/subject.txt
--rw-r--r--   0        0        0     3830 2023-07-30 15:02:55.336964 leprikon-3.5.3/leprikon/templates/leprikon/registration_payments.html
--rw-r--r--   0        0        0    12536 2023-07-30 15:02:55.336964 leprikon-3.5.3/leprikon/templates/leprikon/registration_pdf/subject.rml
--rw-r--r--   0        0        0     4204 2021-02-06 20:07:28.154856 leprikon-3.5.3/leprikon/templates/leprikon/registration_preview.html
--rw-r--r--   0        0        0      438 2022-06-19 21:02:37.435258 leprikon-3.5.3/leprikon/templates/leprikon/registration_received/subject.html
--rw-r--r--   0        0        0      165 2021-06-01 02:09:02.932873 leprikon-3.5.3/leprikon/templates/leprikon/registration_received/subject.subject.txt
--rw-r--r--   0        0        0      433 2022-06-19 21:02:37.435258 leprikon-3.5.3/leprikon/templates/leprikon/registration_received/subject.txt
--rw-r--r--   0        0        0     1031 2021-06-01 05:24:24.368881 leprikon-3.5.3/leprikon/templates/leprikon/registration_recipe.rml
--rw-r--r--   0        0        0      712 2021-06-08 21:18:56.417557 leprikon-3.5.3/leprikon/templates/leprikon/registration_refund_offer/subject.html
--rw-r--r--   0        0        0      180 2021-06-08 20:34:42.425099 leprikon-3.5.3/leprikon/templates/leprikon/registration_refund_offer/subject.subject.txt
--rw-r--r--   0        0        0      575 2021-06-08 21:18:56.417557 leprikon-3.5.3/leprikon/templates/leprikon/registration_refund_offer/subject.txt
--rw-r--r--   0        0        0      152 2021-02-06 20:07:28.154856 leprikon-3.5.3/leprikon/templates/leprikon/registration_refused/subject.html
--rw-r--r--   0        0        0      177 2021-06-01 02:09:02.932873 leprikon-3.5.3/leprikon/templates/leprikon/registration_refused/subject.subject.txt
--rw-r--r--   0        0        0      160 2021-02-06 20:07:28.154856 leprikon-3.5.3/leprikon/templates/leprikon/registration_refused/subject.txt
--rw-r--r--   0        0        0      873 2021-02-06 20:07:28.154856 leprikon-3.5.3/leprikon/templates/leprikon/registrations.html
--rw-r--r--   0        0        0     2387 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/reports/course_payments.html
--rw-r--r--   0        0        0     4667 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/reports/course_payments_status.html
--rw-r--r--   0        0        0     2263 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/reports/course_stats.html
--rw-r--r--   0        0        0     1513 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/reports/debtors.html
--rw-r--r--   0        0        0     2385 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/reports/event_payments.html
--rw-r--r--   0        0        0     4656 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/reports/event_payments_status.html
--rw-r--r--   0        0        0     2127 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/reports/event_stats.html
--rw-r--r--   0        0        0     1934 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/reports/index.html
--rw-r--r--   0        0        0     2405 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/reports/orderable_payments.html
--rw-r--r--   0        0        0     4718 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/reports/orderable_payments_status.html
--rw-r--r--   0        0        0     2151 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/reports/orderable_stats.html
--rw-r--r--   0        0        0     2945 2021-06-01 08:37:09.566968 leprikon-3.5.3/leprikon/templates/leprikon/returned_payment_pdf/recipe.rml
--rw-r--r--   0        0        0     2486 2021-05-31 10:12:28.917535 leprikon-3.5.3/leprikon/templates/leprikon/returned_payment_pdf/subject.rml
--rw-r--r--   0        0        0      136 2021-05-31 12:22:27.052070 leprikon-3.5.3/leprikon/templates/leprikon/returned_payment_received/subject.html
--rw-r--r--   0        0        0      223 2021-06-01 02:09:02.932873 leprikon-3.5.3/leprikon/templates/leprikon/returned_payment_received/subject.subject.txt
--rw-r--r--   0        0        0      145 2021-05-31 12:22:27.052070 leprikon-3.5.3/leprikon/templates/leprikon/returned_payment_received/subject.txt
--rw-r--r--   0        0        0      664 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/schoolyear_form.html
--rw-r--r--   0        0        0       65 2021-02-06 20:07:28.158856 leprikon-3.5.3/leprikon/templates/leprikon/search.txt
--rw-r--r--   0        0        0      765 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/static/bootstrap-datetimepicker.html
--rw-r--r--   0        0        0      286 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/static/bootstrap-multiselect.html
--rw-r--r--   0        0        0      273 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/static/ekko-lightbox.html
--rw-r--r--   0        0        0       35 2021-02-06 20:07:28.158856 leprikon-3.5.3/leprikon/templates/leprikon/subject_form.html
--rw-r--r--   0        0        0       72 2021-08-16 07:31:28.779948 leprikon-3.5.3/leprikon/templates/leprikon/subject_journals.html
--rw-r--r--   0        0        0     1370 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/subject_list.html
--rw-r--r--   0        0        0     4893 2022-09-11 14:45:14.421101 leprikon-3.5.3/leprikon/templates/leprikon/subject_preview.html
--rw-r--r--   0        0        0    28074 2023-07-30 15:02:55.336964 leprikon-3.5.3/leprikon/templates/leprikon/subject_registration_form.html
--rw-r--r--   0        0        0     3542 2021-06-03 02:51:13.941010 leprikon-3.5.3/leprikon/templates/leprikon/summary.html
--rw-r--r--   0        0        0      235 2021-02-06 20:07:28.162856 leprikon-3.5.3/leprikon/templates/leprikon/terms_conditions.html
--rw-r--r--   0        0        0     1959 2021-02-06 20:07:28.162856 leprikon-3.5.3/leprikon/templates/leprikon/timesheet_detail.html
--rw-r--r--   0        0        0      898 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/timesheet_preview.html
--rw-r--r--   0        0        0      189 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/templates/leprikon/timesheetentry_form.html
--rw-r--r--   0        0        0        0 2021-02-06 20:07:28.162856 leprikon-3.5.3/leprikon/templates/leprikon/title.txt
--rw-r--r--   0        0        0      134 2021-02-06 20:07:28.162856 leprikon-3.5.3/leprikon/templates/leprikon/user_create_form_item.html
--rw-r--r--   0        0        0      572 2021-02-06 20:07:28.162856 leprikon-3.5.3/leprikon/templates/leprikon/user_dropdown.html
--rw-r--r--   0        0        0      242 2021-02-06 20:07:28.162856 leprikon-3.5.3/leprikon/templates/leprikon/user_form.html
--rw-r--r--   0        0        0      813 2021-02-06 20:07:28.162856 leprikon-3.5.3/leprikon/templates/leprikon/user_menu.html
--rw-r--r--   0        0        0      283 2021-02-06 20:07:28.162856 leprikon-3.5.3/leprikon/templates/leprikon/widgets/input_option.html
--rw-r--r--   0        0        0      211 2021-02-06 20:07:28.162856 leprikon-3.5.3/leprikon/templates/leprikon/widgets/multiple_input.html
--rw-r--r--   0        0        0      554 2022-06-19 21:02:37.439258 leprikon-3.5.3/leprikon/templates/required_optional_field.html
--rw-r--r--   0        0        0        0 2021-02-06 20:07:28.166856 leprikon-3.5.3/leprikon/templatetags/__init__.py
--rw-r--r--   0        0        0     7364 2023-07-30 15:02:55.336964 leprikon-3.5.3/leprikon/templatetags/leprikon_tags.py
--rw-r--r--   0        0        0      105 2023-01-01 16:24:39.600383 leprikon-3.5.3/leprikon/templatetags/staticfiles.py
--rw-r--r--   0        0        0     5863 2023-07-30 15:02:55.340964 leprikon-3.5.3/leprikon/urls.py
--rw-r--r--   0        0        0     9220 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/utils.py
--rw-r--r--   0        0        0     7516 2021-08-16 07:31:28.779948 leprikon-3.5.3/leprikon/views/__init__.py
--rw-r--r--   0        0        0     1659 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/views/billing_info.py
--rw-r--r--   0        0        0      568 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/views/donation.py
--rw-r--r--   0        0        0     5275 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/views/generic.py
--rw-r--r--   0        0        0     5846 2023-01-09 01:29:07.000459 leprikon-3.5.3/leprikon/views/journals.py
--rw-r--r--   0        0        0      706 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/views/leaders.py
--rw-r--r--   0        0        0     1082 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/views/messages.py
--rw-r--r--   0        0        0     1845 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/views/parents.py
--rw-r--r--   0        0        0     2443 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/views/participants.py
--rw-r--r--   0        0        0     2776 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/views/refundrequest.py
--rw-r--r--   0        0        0     2150 2023-07-30 15:02:55.340964 leprikon-3.5.3/leprikon/views/registrationlink.py
--rw-r--r--   0        0        0     1076 2021-02-15 21:00:52.274425 leprikon-3.5.3/leprikon/views/registrations.py
--rw-r--r--   0        0        0     3486 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/views/reports/__init__.py
--rw-r--r--   0        0        0     9337 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/views/reports/courses.py
--rw-r--r--   0        0        0     2140 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/views/reports/debtors.py
--rw-r--r--   0        0        0     7857 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/views/reports/events.py
--rw-r--r--   0        0        0     8022 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/views/reports/orderables.py
--rw-r--r--   0        0        0      628 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/views/schoolyear.py
--rw-r--r--   0        0        0    12992 2023-07-30 15:02:55.340964 leprikon-3.5.3/leprikon/views/subjects.py
--rw-r--r--   0        0        0     1845 2021-07-30 12:23:56.629387 leprikon-3.5.3/leprikon/views/summaries.py
--rw-r--r--   0        0        0      130 2021-02-06 20:20:39.193125 leprikon-3.5.3/leprikon/views/terms_conditions.py
--rw-r--r--   0        0        0     3175 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/views/timesheets.py
--rw-r--r--   0        0        0     5378 2022-09-11 22:24:07.304086 leprikon-3.5.3/leprikon/views/user.py
--rw-r--r--   0        0        0     2581 2023-08-07 14:40:02.489342 leprikon-3.5.3/pyproject.toml
--rw-r--r--   0        0        0     3271 1970-01-01 00:00:00.000000 leprikon-3.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1483 2021-02-06 20:07:27.966856 leprikon-3.5.4/LICENSE
+-rw-r--r--   0        0        0      698 2021-02-06 20:07:27.966856 leprikon-3.5.4/README.rst
+-rw-r--r--   0        0        0     6359 2023-08-07 14:41:23.641095 leprikon-3.5.4/leprikon/__init__.py
+-rwxr-xr-x   0        0        0      326 2021-02-06 20:20:39.165125 leprikon-3.5.4/leprikon/__main__.py
+-rw-r--r--   0        0        0     2366 2022-09-11 22:24:07.292086 leprikon-3.5.4/leprikon/admin/__init__.py
+-rw-r--r--   0        0        0      194 2021-02-06 20:20:39.169125 leprikon-3.5.4/leprikon/admin/account.py
+-rw-r--r--   0        0        0      341 2023-07-13 19:03:27.661576 leprikon-3.5.4/leprikon/admin/agegroup.py
+-rw-r--r--   0        0        0     1215 2023-07-13 19:03:27.661576 leprikon-3.5.4/leprikon/admin/agreements.py
+-rw-r--r--   0        0        0     3866 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/admin/bulkupdate.py
+-rw-r--r--   0        0        0      316 2023-07-13 19:03:27.665576 leprikon-3.5.4/leprikon/admin/citizenship.py
+-rw-r--r--   0        0        0    13805 2023-08-07 14:39:39.929427 leprikon-3.5.4/leprikon/admin/courses.py
+-rw-r--r--   0        0        0      184 2021-02-06 20:20:39.169125 leprikon-3.5.4/leprikon/admin/department.py
+-rw-r--r--   0        0        0     1280 2021-06-01 08:37:09.562968 leprikon-3.5.4/leprikon/admin/donation.py
+-rw-r--r--   0        0        0     8853 2023-08-07 14:39:39.929427 leprikon-3.5.4/leprikon/admin/events.py
+-rw-r--r--   0        0        0     4695 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/admin/export.py
+-rw-r--r--   0        0        0     8990 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/admin/filters.py
+-rw-r--r--   0        0        0     9088 2023-01-09 01:29:06.992459 leprikon-3.5.4/leprikon/admin/journals.py
+-rw-r--r--   0        0        0      899 2023-01-20 02:25:46.109478 leprikon-3.5.4/leprikon/admin/leprikonsite.py
+-rw-r--r--   0        0        0     8213 2023-01-09 01:29:06.992459 leprikon-3.5.4/leprikon/admin/messages.py
+-rw-r--r--   0        0        0    10131 2023-08-07 14:39:39.929427 leprikon-3.5.4/leprikon/admin/orderables.py
+-rw-r--r--   0        0        0      259 2021-02-06 20:20:39.173125 leprikon-3.5.4/leprikon/admin/organizations.py
+-rw-r--r--   0        0        0     2469 2023-07-13 19:03:27.665576 leprikon-3.5.4/leprikon/admin/pdf.py
+-rw-r--r--   0        0        0      165 2021-02-06 20:20:39.173125 leprikon-3.5.4/leprikon/admin/place.py
+-rw-r--r--   0        0        0      190 2021-02-06 20:20:39.173125 leprikon-3.5.4/leprikon/admin/printsetup.py
+-rw-r--r--   0        0        0      311 2022-06-19 21:02:37.423258 leprikon-3.5.4/leprikon/admin/question.py
+-rw-r--r--   0        0        0     6405 2023-01-11 22:05:01.465080 leprikon-3.5.4/leprikon/admin/refundrequest.py
+-rw-r--r--   0        0        0     5217 2023-07-30 15:02:55.324965 leprikon-3.5.4/leprikon/admin/registrationlink.py
+-rw-r--r--   0        0        0     6294 2023-07-13 19:03:27.665576 leprikon-3.5.4/leprikon/admin/roles.py
+-rw-r--r--   0        0        0      171 2021-02-06 20:20:39.173125 leprikon-3.5.4/leprikon/admin/school.py
+-rw-r--r--   0        0        0     3454 2023-07-13 19:03:27.665576 leprikon-3.5.4/leprikon/admin/schoolyear.py
+-rw-r--r--   0        0        0      399 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/admin/sendmail.py
+-rw-r--r--   0        0        0    45734 2023-07-30 15:02:55.328965 leprikon-3.5.4/leprikon/admin/subjects.py
+-rw-r--r--   0        0        0      310 2023-07-13 19:03:27.665576 leprikon-3.5.4/leprikon/admin/targetgroup.py
+-rw-r--r--   0        0        0     4612 2023-07-13 19:26:09.899255 leprikon-3.5.4/leprikon/admin/timesheets.py
+-rw-r--r--   0        0        0     7470 2023-01-10 14:07:38.306536 leprikon-3.5.4/leprikon/admin/transaction.py
+-rw-r--r--   0        0        0     6951 2023-01-09 01:29:06.996459 leprikon-3.5.4/leprikon/admin/user.py
+-rw-r--r--   0        0        0      635 2022-06-19 21:02:37.423258 leprikon-3.5.4/leprikon/admin/utils.py
+-rw-r--r--   0        0        0        0 2021-02-06 20:07:27.974856 leprikon-3.5.4/leprikon/api/__init__.py
+-rw-r--r--   0        0        0      165 2023-07-13 19:26:09.899255 leprikon-3.5.4/leprikon/api/openapi.py
+-rw-r--r--   0        0        0      948 2023-04-17 11:27:57.487276 leprikon-3.5.4/leprikon/api/serializers.py
+-rw-r--r--   0        0        0      778 2023-07-13 19:26:09.899255 leprikon-3.5.4/leprikon/api/urls.py
+-rw-r--r--   0        0        0     3857 2023-07-30 15:02:55.328965 leprikon-3.5.4/leprikon/api/views.py
+-rw-r--r--   0        0        0     1231 2023-04-17 11:27:57.487276 leprikon-3.5.4/leprikon/apps.py
+-rw-r--r--   0        0        0     1091 2021-02-06 20:20:39.177125 leprikon-3.5.4/leprikon/bankreaders.py
+-rw-r--r--   0        0        0     1263 2023-07-30 15:02:55.328965 leprikon-3.5.4/leprikon/cms_apps.py
+-rw-r--r--   0        0        0     9366 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/cms_menus.py
+-rw-r--r--   0        0        0      150 2021-02-06 20:07:27.978855 leprikon-3.5.4/leprikon/cms_plugins/__init__.py
+-rw-r--r--   0        0        0      440 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/cms_plugins/base.py
+-rw-r--r--   0        0        0     1097 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/cms_plugins/courses.py
+-rw-r--r--   0        0        0     1080 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/cms_plugins/events.py
+-rw-r--r--   0        0        0     1018 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/cms_plugins/leaders.py
+-rw-r--r--   0        0        0     1154 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/cms_plugins/orderables.py
+-rw-r--r--   0        0        0      466 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/cms_plugins/schoolyears.py
+-rw-r--r--   0        0        0      683 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/cms_toolbars.py
+-rw-r--r--   0        0        0      485 2021-02-06 20:20:39.181125 leprikon-3.5.4/leprikon/conf/__init__.py
+-rw-r--r--   0        0        0     4015 2023-01-23 01:36:04.150478 leprikon-3.5.4/leprikon/conf/default_settings.py
+-rw-r--r--   0        0        0     2234 2021-02-06 20:20:39.181125 leprikon-3.5.4/leprikon/cronjobs.py
+-rw-r--r--   0        0        0        0 2021-02-06 20:07:27.982856 leprikon-3.5.4/leprikon/forms/__init__.py
+-rw-r--r--   0        0        0      341 2021-02-06 20:20:39.181125 leprikon-3.5.4/leprikon/forms/billing_info.py
+-rw-r--r--   0        0        0      319 2021-02-15 21:00:52.270425 leprikon-3.5.4/leprikon/forms/confirm.py
+-rw-r--r--   0        0        0     2860 2023-08-01 20:24:04.264870 leprikon-3.5.4/leprikon/forms/courses.py
+-rw-r--r--   0        0        0     2846 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/forms/fields.py
+-rw-r--r--   0        0        0      610 2021-02-15 21:00:52.270425 leprikon-3.5.4/leprikon/forms/form.py
+-rw-r--r--   0        0        0    18999 2023-07-30 15:02:55.328965 leprikon-3.5.4/leprikon/forms/journals.py
+-rw-r--r--   0        0        0      780 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/forms/leaders.py
+-rw-r--r--   0        0        0     2232 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/forms/messages.py
+-rw-r--r--   0        0        0      326 2021-02-06 20:20:39.185125 leprikon-3.5.4/leprikon/forms/parent.py
+-rw-r--r--   0        0        0      716 2021-02-06 20:20:39.185125 leprikon-3.5.4/leprikon/forms/participant.py
+-rw-r--r--   0        0        0     3827 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/forms/refundrequest.py
+-rw-r--r--   0        0        0      446 2022-06-19 21:02:37.423258 leprikon-3.5.4/leprikon/forms/registrationlink.py
+-rw-r--r--   0        0        0        0 2021-02-06 20:07:28.054856 leprikon-3.5.4/leprikon/forms/reports/__init__.py
+-rw-r--r--   0        0        0     1477 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/forms/reports/courses.py
+-rw-r--r--   0        0        0      209 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/forms/reports/debtors.py
+-rw-r--r--   0        0        0     1463 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/forms/reports/events.py
+-rw-r--r--   0        0        0     1503 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/forms/reports/orderables.py
+-rw-r--r--   0        0        0      715 2022-09-11 22:24:07.296086 leprikon-3.5.4/leprikon/forms/schoolyear.py
+-rw-r--r--   0        0        0    39013 2023-08-01 20:10:29.970532 leprikon-3.5.4/leprikon/forms/subjects.py
+-rw-r--r--   0        0        0     3521 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/forms/timesheets.py
+-rw-r--r--   0        0        0     4245 2023-04-17 11:27:57.487276 leprikon-3.5.4/leprikon/forms/user.py
+-rw-r--r--   0        0        0     1088 2022-06-19 21:02:37.427258 leprikon-3.5.4/leprikon/forms/widgets.py
+-rw-r--r--   0        0        0      209 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/gettext_overrides.py
+-rw-r--r--   0        0        0    77353 2023-08-01 20:22:30.958943 leprikon-3.5.4/leprikon/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   141305 2023-08-01 20:22:38.343558 leprikon-3.5.4/leprikon/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      323 2022-09-04 23:40:36.644492 leprikon-3.5.4/leprikon/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   111732 2022-09-04 22:12:01.810032 leprikon-3.5.4/leprikon/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2021-02-06 20:07:28.070855 leprikon-3.5.4/leprikon/management/__init__.py
+-rw-r--r--   0        0        0        0 2021-02-06 20:07:28.070855 leprikon-3.5.4/leprikon/management/commands/__init__.py
+-rw-r--r--   0        0        0     4121 2022-06-19 21:02:37.431258 leprikon-3.5.4/leprikon/middleware.py
+-rw-r--r--   0        0        0    59583 2023-01-23 01:36:04.150478 leprikon-3.5.4/leprikon/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1851 2021-02-06 20:07:28.070855 leprikon-3.5.4/leprikon/migrations/0002_initial_data.py
+-rw-r--r--   0        0        0     1954 2021-02-06 20:07:28.070855 leprikon-3.5.4/leprikon/migrations/0003_managers.py
+-rw-r--r--   0        0        0      345 2021-02-06 20:07:28.070855 leprikon-3.5.4/leprikon/migrations/0004_multiple_registrations.py
+-rw-r--r--   0        0        0      879 2021-02-06 20:07:28.070855 leprikon-3.5.4/leprikon/migrations/0005_subjectregistration_variable_symbol.py
+-rw-r--r--   0        0        0     1049 2021-02-06 20:07:28.070855 leprikon-3.5.4/leprikon/migrations/0006_discount_periods.py
+-rw-r--r--   0        0        0      864 2021-02-06 20:07:28.070855 leprikon-3.5.4/leprikon/migrations/0007_bill_print_setup.py
+-rw-r--r--   0        0        0      449 2021-02-06 20:07:28.070855 leprikon-3.5.4/leprikon/migrations/0008_leprikonsite_company_name.py
+-rw-r--r--   0        0        0      656 2021-02-06 20:07:28.070855 leprikon-3.5.4/leprikon/migrations/0009_subjectpayment_received_by.py
+-rw-r--r--   0        0        0      449 2021-02-06 20:07:28.070855 leprikon-3.5.4/leprikon/migrations/0010_subject_code.py
+-rw-r--r--   0        0        0      457 2021-02-06 20:07:28.070855 leprikon-3.5.4/leprikon/migrations/0011_subjectregistration_payment_requested.py
+-rw-r--r--   0        0        0     1720 2023-08-01 20:22:11.113519 leprikon-3.5.4/leprikon/migrations/0012_subject_variants.py
+-rw-r--r--   0        0        0      549 2021-02-06 20:07:28.070855 leprikon-3.5.4/leprikon/migrations/0013_drop_insurance.py
+-rw-r--r--   0        0        0      472 2021-02-06 20:07:28.070855 leprikon-3.5.4/leprikon/migrations/0014_variable_symbol.py
+-rw-r--r--   0        0        0     4137 2021-02-06 20:07:28.070855 leprikon-3.5.4/leprikon/migrations/0015_school_year_divisions.py
+-rw-r--r--   0        0        0     1191 2021-02-06 20:07:28.070855 leprikon-3.5.4/leprikon/migrations/0016_school_year_divisions_cleanup.py
+-rw-r--r--   0        0        0     3919 2023-07-13 19:03:27.669576 leprikon-3.5.4/leprikon/migrations/0017_citizenship.py
+-rw-r--r--   0        0        0      475 2021-02-06 20:07:28.070855 leprikon-3.5.4/leprikon/migrations/0018_citizenship_cleanup.py
+-rw-r--r--   0        0        0     3040 2021-02-06 20:07:28.070855 leprikon-3.5.4/leprikon/migrations/0019_department.py
+-rw-r--r--   0        0        0     1377 2021-02-06 20:07:28.070855 leprikon-3.5.4/leprikon/migrations/0020_agreements.py
+-rw-r--r--   0        0        0     1532 2021-02-06 20:07:28.074856 leprikon-3.5.4/leprikon/migrations/0021_user_agreement.py
+-rw-r--r--   0        0        0      671 2021-02-06 20:07:28.074856 leprikon-3.5.4/leprikon/migrations/0022_bankreader.py
+-rw-r--r--   0        0        0     2506 2021-02-06 20:07:28.074856 leprikon-3.5.4/leprikon/migrations/0023_accountclosure.py
+-rw-r--r--   0        0        0      504 2021-02-06 20:07:28.074856 leprikon-3.5.4/leprikon/migrations/0024_subjectregistration_note.py
+-rw-r--r--   0        0        0     5224 2021-02-06 20:07:28.074856 leprikon-3.5.4/leprikon/migrations/0025_agreements.py
+-rw-r--r--   0        0        0      942 2021-02-06 20:07:28.074856 leprikon-3.5.4/leprikon/migrations/0026_online_payments.py
+-rw-r--r--   0        0        0     2243 2021-02-06 20:07:28.074856 leprikon-3.5.4/leprikon/migrations/0027_journals.py
+-rw-r--r--   0        0        0      517 2021-02-06 20:07:28.074856 leprikon-3.5.4/leprikon/migrations/0028_agegroups.py
+-rw-r--r--   0        0        0      646 2021-02-06 20:07:28.074856 leprikon-3.5.4/leprikon/migrations/0029_payment_restrictions.py
+-rw-r--r--   0        0        0      716 2021-02-06 20:07:28.074856 leprikon-3.5.4/leprikon/migrations/0030_agreements.py
+-rw-r--r--   0        0        0     2208 2021-02-06 20:07:28.074856 leprikon-3.5.4/leprikon/migrations/0031_registration_questions_agreements.py
+-rw-r--r--   0        0        0    15532 2021-02-06 20:07:28.074856 leprikon-3.5.4/leprikon/migrations/0032_registration_participants_groups.py
+-rw-r--r--   0        0        0     4196 2021-02-06 20:07:28.074856 leprikon-3.5.4/leprikon/migrations/0033_target_groups.py
+-rw-r--r--   0        0        0     9741 2022-09-11 14:45:14.421101 leprikon-3.5.4/leprikon/migrations/0034_subject_registration_group.py
+-rw-r--r--   0        0        0     1807 2021-02-06 20:07:28.078856 leprikon-3.5.4/leprikon/migrations/0035_on_delete.py
+-rw-r--r--   0        0        0     1220 2021-02-06 20:07:28.078856 leprikon-3.5.4/leprikon/migrations/0036_participants_instructed.py
+-rw-r--r--   0        0        0      703 2021-02-06 20:07:28.078856 leprikon-3.5.4/leprikon/migrations/0037_message_sender.py
+-rw-r--r--   0        0        0     6559 2021-02-06 20:07:28.078856 leprikon-3.5.4/leprikon/migrations/0038_organizations.py
+-rw-r--r--   0        0        0     4941 2021-02-06 20:07:28.078856 leprikon-3.5.4/leprikon/migrations/0039_editable_texts.py
+-rw-r--r--   0        0        0     1827 2021-02-06 20:07:28.078856 leprikon-3.5.4/leprikon/migrations/0040_due_dates.py
+-rw-r--r--   0        0        0     2946 2021-02-06 20:07:28.082856 leprikon-3.5.4/leprikon/migrations/0041_billing_info.py
+-rw-r--r--   0        0        0     1207 2021-02-06 20:07:28.082856 leprikon-3.5.4/leprikon/migrations/0042_chat_group_types.py
+-rw-r--r--   0        0        0     1960 2021-02-06 20:07:28.082856 leprikon-3.5.4/leprikon/migrations/0043_registration_links.py
+-rw-r--r--   0        0        0     2153 2021-02-06 20:07:28.082856 leprikon-3.5.4/leprikon/migrations/0044_billinginfo_contacts.py
+-rw-r--r--   0        0        0      527 2021-02-06 20:07:28.082856 leprikon-3.5.4/leprikon/migrations/0045_registration_slug.py
+-rw-r--r--   0        0        0     3632 2021-02-06 20:07:28.082856 leprikon-3.5.4/leprikon/migrations/0046_attachment_events.py
+-rw-r--r--   0        0        0     6061 2021-02-06 20:07:28.086856 leprikon-3.5.4/leprikon/migrations/0047_pr_print_setup.py
+-rw-r--r--   0        0        0     2700 2021-02-06 20:07:28.086856 leprikon-3.5.4/leprikon/migrations/0048_birth_date.py
+-rw-r--r--   0        0        0      999 2021-02-06 20:07:28.086856 leprikon-3.5.4/leprikon/migrations/0049_target_groups_fix.py
+-rw-r--r--   0        0        0    11512 2022-06-19 21:02:37.431258 leprikon-3.5.4/leprikon/migrations/0050_orderables.py
+-rw-r--r--   0        0        0      546 2021-02-06 20:07:28.086856 leprikon-3.5.4/leprikon/migrations/0051_registration_group_name.py
+-rw-r--r--   0        0        0      762 2021-02-06 20:07:28.086856 leprikon-3.5.4/leprikon/migrations/0052_payment_notification_sent.py
+-rw-r--r--   0        0        0     2528 2021-02-06 20:07:28.090856 leprikon-3.5.4/leprikon/migrations/0053_registration_dates_by.py
+-rw-r--r--   0        0        0      460 2021-02-06 20:07:28.090856 leprikon-3.5.4/leprikon/migrations/0054_registration_dates_by_cleanup.py
+-rw-r--r--   0        0        0     1020 2021-02-06 20:07:28.090856 leprikon-3.5.4/leprikon/migrations/0055_schoolyearblockplugin.py
+-rw-r--r--   0        0        0     4108 2021-02-06 20:07:28.090856 leprikon-3.5.4/leprikon/migrations/0056_registration_period.py
+-rw-r--r--   0        0        0      739 2021-02-06 20:07:28.094856 leprikon-3.5.4/leprikon/migrations/0057_registration_period.py
+-rw-r--r--   0        0        0     1229 2021-02-06 20:07:28.094856 leprikon-3.5.4/leprikon/migrations/0058_agegroup_min_max_age.py
+-rw-r--r--   0        0        0     5253 2021-07-30 12:23:56.621387 leprikon-3.5.4/leprikon/migrations/0059_transactions_data.py
+-rw-r--r--   0        0        0    12344 2021-06-03 01:45:58.168248 leprikon-3.5.4/leprikon/migrations/0060_transactions.py
+-rw-r--r--   0        0        0     2055 2021-06-03 02:51:13.941010 leprikon-3.5.4/leprikon/migrations/0061_refundrequest.py
+-rw-r--r--   0        0        0     4102 2021-06-08 21:18:56.417557 leprikon-3.5.4/leprikon/migrations/0062_refund_offers.py
+-rw-r--r--   0        0        0     7724 2021-08-31 21:32:49.271400 leprikon-3.5.4/leprikon/migrations/0063_journals.py
+-rw-r--r--   0        0        0     1127 2021-10-26 23:31:48.142344 leprikon-3.5.4/leprikon/migrations/0064_journals_cleanup.py
+-rw-r--r--   0        0        0     1600 2022-06-19 21:02:37.431258 leprikon-3.5.4/leprikon/migrations/0065_subject_type_page.py
+-rw-r--r--   0        0        0      453 2022-06-19 21:02:37.431258 leprikon-3.5.4/leprikon/migrations/0066_subject_type_slug_unique.py
+-rw-r--r--   0        0        0      528 2022-06-19 21:02:37.431258 leprikon-3.5.4/leprikon/migrations/0067_remove_rocketchat.py
+-rw-r--r--   0        0        0      518 2022-06-19 21:02:37.431258 leprikon-3.5.4/leprikon/migrations/0068_participant_answers.py
+-rw-r--r--   0        0        0     2329 2023-01-20 01:19:05.975668 leprikon-3.5.4/leprikon/migrations/0069_question_slug.py
+-rw-r--r--   0        0        0     1851 2023-01-20 01:19:05.975668 leprikon-3.5.4/leprikon/migrations/0070_decision_print_setup.py
+-rw-r--r--   0        0        0      746 2022-09-04 23:40:36.644492 leprikon-3.5.4/leprikon/migrations/0071_transaction_amount.py
+-rw-r--r--   0        0        0     9100 2022-09-11 15:35:00.764956 leprikon-3.5.4/leprikon/migrations/0072_prices.py
+-rw-r--r--   0        0        0     3555 2023-01-23 01:36:04.150478 leprikon-3.5.4/leprikon/migrations/0073_add_limit_choices_to.py
+-rw-r--r--   0        0        0     1311 2023-01-09 01:29:06.996459 leprikon-3.5.4/leprikon/migrations/0074_schoolyear_period_order.py
+-rw-r--r--   0        0        0     3311 2023-07-30 15:02:55.328965 leprikon-3.5.4/leprikon/migrations/0075_journal_school_year_division.py
+-rw-r--r--   0        0        0     1603 2023-01-09 01:29:06.996459 leprikon-3.5.4/leprikon/migrations/0076_journalentry_period.py
+-rw-r--r--   0        0        0      482 2023-01-23 01:36:04.150478 leprikon-3.5.4/leprikon/migrations/0077_place_description.py
+-rw-r--r--   0        0        0     1840 2023-07-13 19:03:27.669576 leprikon-3.5.4/leprikon/migrations/0078_delete_coursevariant.py
+-rw-r--r--   0        0        0     8301 2023-08-01 20:10:29.970532 leprikon-3.5.4/leprikon/migrations/0079_mandatory_subject_variants.py
+-rw-r--r--   0        0        0        0 2021-02-06 20:07:28.094856 leprikon-3.5.4/leprikon/migrations/__init__.py
+-rw-r--r--   0        0        0      463 2021-06-03 02:51:13.941010 leprikon-3.5.4/leprikon/models/__init__.py
+-rw-r--r--   0        0        0      641 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/models/account.py
+-rw-r--r--   0        0        0      793 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/models/agegroup.py
+-rw-r--r--   0        0        0     1553 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/models/agreements.py
+-rw-r--r--   0        0        0      540 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/models/citizenship.py
+-rw-r--r--   0        0        0    17737 2023-07-30 15:02:55.332965 leprikon-3.5.4/leprikon/models/courses.py
+-rw-r--r--   0        0        0      616 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/models/department.py
+-rw-r--r--   0        0        0      704 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/models/donation.py
+-rw-r--r--   0        0        0    12356 2023-07-30 15:02:55.332965 leprikon-3.5.4/leprikon/models/events.py
+-rw-r--r--   0        0        0     5763 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/models/fields.py
+-rw-r--r--   0        0        0    10471 2023-07-30 15:02:55.332965 leprikon-3.5.4/leprikon/models/journals.py
+-rw-r--r--   0        0        0     3367 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/models/leprikonsite.py
+-rw-r--r--   0        0        0     4316 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/models/messages.py
+-rw-r--r--   0        0        0    12852 2023-07-30 15:02:55.332965 leprikon-3.5.4/leprikon/models/orderables.py
+-rw-r--r--   0        0        0     1896 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/models/organizations.py
+-rw-r--r--   0        0        0     4129 2023-07-13 19:03:27.669576 leprikon-3.5.4/leprikon/models/pdfmail.py
+-rw-r--r--   0        0        0      714 2023-01-23 01:36:04.150478 leprikon-3.5.4/leprikon/models/place.py
+-rw-r--r--   0        0        0     2183 2023-07-13 19:03:27.669576 leprikon-3.5.4/leprikon/models/printsetup.py
+-rw-r--r--   0        0        0     2093 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/models/question.py
+-rw-r--r--   0        0        0     1625 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/models/refundrequest.py
+-rw-r--r--   0        0        0     1730 2023-07-30 15:02:55.332965 leprikon-3.5.4/leprikon/models/registrationlink.py
+-rw-r--r--   0        0        0    12114 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/models/roles.py
+-rw-r--r--   0        0        0      894 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/models/school.py
+-rw-r--r--   0        0        0     5005 2023-01-09 01:29:06.996459 leprikon-3.5.4/leprikon/models/schoolyear.py
+-rw-r--r--   0        0        0      639 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/models/startend.py
+-rw-r--r--   0        0        0    68416 2023-08-01 20:13:53.729874 leprikon-3.5.4/leprikon/models/subjects.py
+-rw-r--r--   0        0        0      626 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/models/targetgroup.py
+-rw-r--r--   0        0        0     1482 2021-06-03 03:12:18.850194 leprikon-3.5.4/leprikon/models/test_utils.py
+-rw-r--r--   0        0        0     2787 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/models/times.py
+-rw-r--r--   0        0        0     5592 2023-01-20 01:19:05.979668 leprikon-3.5.4/leprikon/models/timesheets.py
+-rw-r--r--   0        0        0     9259 2023-01-20 01:19:05.979668 leprikon-3.5.4/leprikon/models/transaction.py
+-rw-r--r--   0        0        0      439 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/models/useragreement.py
+-rw-r--r--   0        0        0     9133 2023-07-30 15:02:55.336964 leprikon-3.5.4/leprikon/models/utils.py
+-rw-r--r--   0        0        0      127 2021-02-06 20:07:28.098856 leprikon-3.5.4/leprikon/search_indexes/__init__.py
+-rw-r--r--   0        0        0      682 2021-02-06 20:20:39.189125 leprikon-3.5.4/leprikon/search_indexes/base.py
+-rw-r--r--   0        0        0      143 2021-02-06 20:20:39.189125 leprikon-3.5.4/leprikon/search_indexes/courses.py
+-rw-r--r--   0        0        0      139 2021-02-06 20:20:39.189125 leprikon-3.5.4/leprikon/search_indexes/events.py
+-rw-r--r--   0        0        0      155 2021-02-06 20:20:39.189125 leprikon-3.5.4/leprikon/search_indexes/orderables.py
+-rw-r--r--   0        0        0        0 2021-02-06 20:07:28.102856 leprikon-3.5.4/leprikon/site/__init__.py
+-rw-r--r--   0        0        0    16830 2023-07-30 15:02:55.336964 leprikon-3.5.4/leprikon/site/settings.py
+-rw-r--r--   0        0        0     1761 2023-07-17 19:51:19.009803 leprikon-3.5.4/leprikon/site/urls.py
+-rw-r--r--   0        0        0      458 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/site/wsgi.py
+-rw-r--r--   0        0        0      566 2023-01-20 01:19:05.979668 leprikon-3.5.4/leprikon/static/admin/css/scrollbars.css
+-rw-r--r--   0        0        0     5994 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/static/admin/js/admin/RelatedObjectLookups.js
+-rw-r--r--   0        0        0    10366 2021-02-06 20:07:28.102856 leprikon-3.5.4/leprikon/static/favicon.ico
+-rw-r--r--   0        0        0     3153 2021-02-06 20:07:28.102856 leprikon-3.5.4/leprikon/static/leprikon/css/colors.css
+-rw-r--r--   0        0        0     4472 2021-02-06 20:07:28.102856 leprikon-3.5.4/leprikon/static/leprikon/css/layout.css
+-rw-r--r--   0        0        0     1138 2021-02-06 20:07:28.102856 leprikon-3.5.4/leprikon/static/leprikon/css/registrations.changelist.css
+-rw-r--r--   0        0        0   705684 2021-02-06 20:07:28.118856 leprikon-3.5.4/leprikon/static/leprikon/fonts/DejaVuSans-Bold.ttf
+-rw-r--r--   0        0        0   643292 2021-02-06 20:07:28.126856 leprikon-3.5.4/leprikon/static/leprikon/fonts/DejaVuSans-BoldOblique.ttf
+-rw-r--r--   0        0        0   635416 2021-02-06 20:07:28.134856 leprikon-3.5.4/leprikon/static/leprikon/fonts/DejaVuSans-Oblique.ttf
+-rw-r--r--   0        0        0   757076 2021-02-06 20:07:28.138856 leprikon-3.5.4/leprikon/static/leprikon/fonts/DejaVuSans.ttf
+-rw-r--r--   0        0        0    83151 2021-02-06 20:07:28.138856 leprikon-3.5.4/leprikon/static/leprikon/img/leprikon-kuk-l.png
+-rw-r--r--   0        0        0    51531 2021-02-06 20:07:28.138856 leprikon-3.5.4/leprikon/static/leprikon/img/logo-horizontal.png
+-rw-r--r--   0        0        0   200727 2021-02-06 20:07:28.138856 leprikon-3.5.4/leprikon/static/leprikon/img/logo.png
+-rw-r--r--   0        0        0      522 2021-02-06 20:07:28.138856 leprikon-3.5.4/leprikon/static/leprikon/js/Popup.js
+-rw-r--r--   0        0        0     1517 2022-06-19 21:02:37.435258 leprikon-3.5.4/leprikon/static/leprikon/js/required_optional_field.js
+-rw-r--r--   0        0        0      175 2023-01-09 01:29:07.000459 leprikon-3.5.4/leprikon/staticfiles.py
+-rw-r--r--   0        0        0      727 2021-02-06 20:07:28.142856 leprikon-3.5.4/leprikon/templates/admin/base.html
+-rw-r--r--   0        0        0     1175 2021-02-06 20:07:28.142856 leprikon-3.5.4/leprikon/templates/admin/change_list.html
+-rw-r--r--   0        0        0     1570 2021-02-06 20:07:28.142856 leprikon-3.5.4/leprikon/templates/admin/change_list_results.html
+-rw-r--r--   0        0        0     1589 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/templates/admin/inc/branding.html
+-rw-r--r--   0        0        0       96 2021-02-06 20:07:28.142856 leprikon-3.5.4/leprikon/templates/admin/inc/extrahead.html
+-rw-r--r--   0        0        0      134 2021-02-06 20:07:28.142856 leprikon-3.5.4/leprikon/templates/admin/leprikon/app_index.html
+-rw-r--r--   0        0        0      207 2021-02-06 20:07:28.142856 leprikon-3.5.4/leprikon/templates/admin/leprikon/coursediscount/popup_response.html
+-rw-r--r--   0        0        0      561 2021-06-01 05:03:47.670256 leprikon-3.5.4/leprikon/templates/admin/leprikon/donation/change_form.html
+-rw-r--r--   0        0        0      207 2021-02-06 20:07:28.142856 leprikon-3.5.4/leprikon/templates/admin/leprikon/eventdiscount/popup_response.html
+-rw-r--r--   0        0        0      563 2021-02-06 20:07:28.142856 leprikon-3.5.4/leprikon/templates/admin/leprikon/message/add_recipients.html
+-rw-r--r--   0        0        0      460 2021-02-06 20:07:28.142856 leprikon-3.5.4/leprikon/templates/admin/leprikon/messagerecipient/change_list.html
+-rw-r--r--   0        0        0     2425 2021-02-06 20:07:28.142856 leprikon-3.5.4/leprikon/templates/admin/leprikon/messagerecipient/send_mails.html
+-rw-r--r--   0        0        0      207 2021-02-06 20:07:28.142856 leprikon-3.5.4/leprikon/templates/admin/leprikon/orderablediscount/popup_response.html
+-rw-r--r--   0        0        0      560 2021-06-01 05:03:47.670256 leprikon-3.5.4/leprikon/templates/admin/leprikon/subjectreceivedpayment/change_form.html
+-rw-r--r--   0        0        0      207 2021-06-01 05:03:47.670256 leprikon-3.5.4/leprikon/templates/admin/leprikon/subjectreceivedpayment/popup_response.html
+-rw-r--r--   0        0        0      560 2021-06-01 05:03:47.670256 leprikon-3.5.4/leprikon/templates/admin/leprikon/subjectreturnedpayment/change_form.html
+-rw-r--r--   0        0        0      207 2021-05-31 17:36:24.566151 leprikon-3.5.4/leprikon/templates/admin/leprikon/subjectreturnedpayment/popup_response.html
+-rw-r--r--   0        0        0        0 2021-02-06 20:07:28.142856 leprikon-3.5.4/leprikon/templates/auth/widgets/read_only_password_hash.html
+-rw-r--r--   0        0        0      257 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/templates/cms/toolbar/items/logo.html
+-rw-r--r--   0        0        0     1180 2021-02-06 20:07:28.142856 leprikon-3.5.4/leprikon/templates/leprikon/admin/action_form.html
+-rw-r--r--   0        0        0     1170 2023-01-09 01:29:07.000459 leprikon-3.5.4/leprikon/templates/leprikon/admin/bulk_update_form.html
+-rw-r--r--   0        0        0     2978 2021-08-16 07:31:28.779948 leprikon-3.5.4/leprikon/templates/leprikon/admin/dashboard.html
+-rw-r--r--   0        0        0     1235 2021-02-06 20:07:28.142856 leprikon-3.5.4/leprikon/templates/leprikon/admin/merge.html
+-rw-r--r--   0        0        0     1077 2021-02-06 20:07:28.142856 leprikon-3.5.4/leprikon/templates/leprikon/admin/send_message.html
+-rw-r--r--   0        0        0     1296 2021-02-06 20:07:28.142856 leprikon-3.5.4/leprikon/templates/leprikon/alternating.html
+-rw-r--r--   0        0        0     3431 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/templates/leprikon/base.html
+-rw-r--r--   0        0        0     1089 2021-02-06 20:07:28.142856 leprikon-3.5.4/leprikon/templates/leprikon/billing_info_preview.html
+-rw-r--r--   0        0        0       73 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/cms/course/default.html
+-rw-r--r--   0        0        0      142 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/cms/course_list/default.html
+-rw-r--r--   0        0        0      326 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/cms/course_list/grouped.html
+-rw-r--r--   0        0        0     1368 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/templates/leprikon/cms/course_list_filtered.html
+-rw-r--r--   0        0        0       70 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/cms/event/default.html
+-rw-r--r--   0        0        0      139 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/cms/event_list/default.html
+-rw-r--r--   0        0        0      324 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/cms/event_list/grouped.html
+-rw-r--r--   0        0        0     1001 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/templates/leprikon/cms/event_list_filtered.html
+-rw-r--r--   0        0        0       73 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/cms/leader/default.html
+-rw-r--r--   0        0        0     1694 2023-08-07 14:41:23.641095 leprikon-3.5.4/leprikon/templates/leprikon/cms/leader_list/default.html
+-rw-r--r--   0        0        0     1086 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/templates/leprikon/cms/leader_list_filtered.html
+-rw-r--r--   0        0        0       82 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/cms/orderable/default.html
+-rw-r--r--   0        0        0      151 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/cms/orderable_list/default.html
+-rw-r--r--   0        0        0      332 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/cms/orderable_list/grouped.html
+-rw-r--r--   0        0        0     1013 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/templates/leprikon/cms/orderable_list_filtered.html
+-rw-r--r--   0        0        0      206 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/cms/school_year_block.html
+-rw-r--r--   0        0        0      199 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/cms.html
+-rw-r--r--   0        0        0      769 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/confirm_form.html
+-rw-r--r--   0        0        0      224 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/course_detail.html
+-rw-r--r--   0        0        0       65 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/course_preview.html
+-rw-r--r--   0        0        0     1198 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/course_registrations.html
+-rw-r--r--   0        0        0       35 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/default.html
+-rw-r--r--   0        0        0     2470 2021-06-01 02:09:02.932873 leprikon-3.5.4/leprikon/templates/leprikon/donation_pdf/default.rml
+-rw-r--r--   0        0        0     2701 2021-06-01 05:24:24.368881 leprikon-3.5.4/leprikon/templates/leprikon/donation_pdf/recipe.rml
+-rw-r--r--   0        0        0      937 2021-06-01 09:11:38.676158 leprikon-3.5.4/leprikon/templates/leprikon/donations.html
+-rw-r--r--   0        0        0      223 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/event_detail.html
+-rw-r--r--   0        0        0       64 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/event_preview.html
+-rw-r--r--   0        0        0     1187 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/event_registrations.html
+-rw-r--r--   0        0        0      732 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/filter_form.html
+-rw-r--r--   0        0        0     1991 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/templates/leprikon/filtered_subject_list.html
+-rw-r--r--   0        0        0     2198 2021-08-31 20:34:46.158520 leprikon-3.5.4/leprikon/templates/leprikon/form.html
+-rw-r--r--   0        0        0      254 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/form_inline_item.html
+-rw-r--r--   0        0        0      493 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/form_item.html
+-rw-r--r--   0        0        0      604 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/form_item_checkbox.html
+-rw-r--r--   0        0        0      368 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/form_item_fullwidth.html
+-rw-r--r--   0        0        0     7105 2023-01-09 01:29:07.000459 leprikon-3.5.4/leprikon/templates/leprikon/invoices.xml
+-rw-r--r--   0        0        0      531 2022-09-11 22:24:07.300086 leprikon-3.5.4/leprikon/templates/leprikon/journal_form.html
+-rw-r--r--   0        0        0    12058 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/journal_journal.html
+-rw-r--r--   0        0        0     2271 2021-08-16 07:31:28.779948 leprikon-3.5.4/leprikon/templates/leprikon/journal_journal_pdf/default.rml
+-rw-r--r--   0        0        0     2023 2022-06-19 21:02:37.435258 leprikon-3.5.4/leprikon/templates/leprikon/journal_preview.html
+-rw-r--r--   0        0        0     2481 2023-07-30 15:02:55.336964 leprikon-3.5.4/leprikon/templates/leprikon/journalentry_form.html
+-rw-r--r--   0        0        0      189 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/journalleaderentry_form.html
+-rw-r--r--   0        0        0     1006 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/leader_list.html
+-rw-r--r--   0        0        0     2220 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/leader_preview.html
+-rw-r--r--   0        0        0      553 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/leader_summary.html
+-rw-r--r--   0        0        0      743 2021-02-06 20:07:28.146856 leprikon-3.5.4/leprikon/templates/leprikon/list.html
+-rw-r--r--   0        0        0     4959 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/login.html
+-rw-r--r--   0        0        0      543 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/menu.html
+-rw-r--r--   0        0        0      222 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/message_list.html
+-rw-r--r--   0        0        0      320 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/message_mail.html
+-rw-r--r--   0        0        0      222 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/message_mail.txt
+-rw-r--r--   0        0        0      735 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/messagerecipient_detail.html
+-rw-r--r--   0        0        0      586 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/messages_table.html
+-rw-r--r--   0        0        0     1021 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/modal_messages.html
+-rw-r--r--   0        0        0      227 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/orderable_detail.html
+-rw-r--r--   0        0        0       68 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/orderable_preview.html
+-rw-r--r--   0        0        0     1231 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/orderable_registrations.html
+-rw-r--r--   0        0        0      898 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/pagination.html
+-rw-r--r--   0        0        0      915 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/parent_preview.html
+-rw-r--r--   0        0        0     1742 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/participant_preview.html
+-rw-r--r--   0        0        0      443 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/participants.html
+-rw-r--r--   0        0        0       35 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/password.html
+-rw-r--r--   0        0        0      222 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/password_change_done.html
+-rw-r--r--   0        0        0       35 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/password_reset.html
+-rw-r--r--   0        0        0      368 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/password_reset_complete.html
+-rw-r--r--   0        0        0       35 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/password_reset_confirm.html
+-rw-r--r--   0        0        0      439 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/password_reset_done.html
+-rw-r--r--   0        0        0      592 2021-02-06 20:07:28.150856 leprikon-3.5.4/leprikon/templates/leprikon/password_reset_email.html
+-rw-r--r--   0        0        0     1617 2021-06-01 22:52:10.045174 leprikon-3.5.4/leprikon/templates/leprikon/payments.html
+-rw-r--r--   0        0        0     2936 2021-06-01 08:37:09.562968 leprikon-3.5.4/leprikon/templates/leprikon/received_payment_pdf/recipe.rml
+-rw-r--r--   0        0        0     2486 2021-06-01 08:37:09.562968 leprikon-3.5.4/leprikon/templates/leprikon/received_payment_pdf/subject.rml
+-rw-r--r--   0        0        0      136 2021-06-01 08:37:09.566968 leprikon-3.5.4/leprikon/templates/leprikon/received_payment_received/subject.html
+-rw-r--r--   0        0        0      223 2021-06-01 08:37:09.566968 leprikon-3.5.4/leprikon/templates/leprikon/received_payment_received/subject.subject.txt
+-rw-r--r--   0        0        0      145 2021-06-01 08:37:09.566968 leprikon-3.5.4/leprikon/templates/leprikon/received_payment_received/subject.txt
+-rw-r--r--   0        0        0      153 2021-02-06 20:07:28.154856 leprikon-3.5.4/leprikon/templates/leprikon/registration_approved/subject.html
+-rw-r--r--   0        0        0      178 2021-06-01 02:09:02.932873 leprikon-3.5.4/leprikon/templates/leprikon/registration_approved/subject.subject.txt
+-rw-r--r--   0        0        0      161 2021-02-06 20:07:28.154856 leprikon-3.5.4/leprikon/templates/leprikon/registration_approved/subject.txt
+-rw-r--r--   0        0        0      153 2021-02-06 20:07:28.154856 leprikon-3.5.4/leprikon/templates/leprikon/registration_canceled/subject.html
+-rw-r--r--   0        0        0      178 2021-06-01 02:09:02.932873 leprikon-3.5.4/leprikon/templates/leprikon/registration_canceled/subject.subject.txt
+-rw-r--r--   0        0        0      161 2021-02-06 20:07:28.154856 leprikon-3.5.4/leprikon/templates/leprikon/registration_canceled/subject.txt
+-rw-r--r--   0        0        0     5431 2022-06-19 23:56:58.526604 leprikon-3.5.4/leprikon/templates/leprikon/registration_decision/subject.rml
+-rw-r--r--   0        0        0     6268 2021-02-06 20:07:28.154856 leprikon-3.5.4/leprikon/templates/leprikon/registration_details.html
+-rw-r--r--   0        0        0     1209 2022-08-09 07:23:11.034741 leprikon-3.5.4/leprikon/templates/leprikon/registration_links.html
+-rw-r--r--   0        0        0      610 2021-06-08 20:34:42.425099 leprikon-3.5.4/leprikon/templates/leprikon/registration_mail_details.html
+-rw-r--r--   0        0        0      534 2021-06-08 20:34:42.425099 leprikon-3.5.4/leprikon/templates/leprikon/registration_mail_details.txt
+-rw-r--r--   0        0        0      300 2021-02-06 20:07:28.154856 leprikon-3.5.4/leprikon/templates/leprikon/registration_mail_footer.html
+-rw-r--r--   0        0        0      189 2021-02-06 20:07:28.154856 leprikon-3.5.4/leprikon/templates/leprikon/registration_mail_footer.txt
+-rw-r--r--   0        0        0      427 2021-08-16 07:31:28.779948 leprikon-3.5.4/leprikon/templates/leprikon/registration_participant_presence.html
+-rw-r--r--   0        0        0     1568 2021-02-06 20:07:28.154856 leprikon-3.5.4/leprikon/templates/leprikon/registration_payment_request/subject.html
+-rw-r--r--   0        0        0    12348 2021-02-06 20:07:28.154856 leprikon-3.5.4/leprikon/templates/leprikon/registration_payment_request/subject.rml
+-rw-r--r--   0        0        0      183 2021-06-01 02:09:02.932873 leprikon-3.5.4/leprikon/templates/leprikon/registration_payment_request/subject.subject.txt
+-rw-r--r--   0        0        0     1172 2021-02-06 20:07:28.154856 leprikon-3.5.4/leprikon/templates/leprikon/registration_payment_request/subject.txt
+-rw-r--r--   0        0        0     3830 2023-07-30 15:02:55.336964 leprikon-3.5.4/leprikon/templates/leprikon/registration_payments.html
+-rw-r--r--   0        0        0    12536 2023-07-30 15:02:55.336964 leprikon-3.5.4/leprikon/templates/leprikon/registration_pdf/subject.rml
+-rw-r--r--   0        0        0     4204 2021-02-06 20:07:28.154856 leprikon-3.5.4/leprikon/templates/leprikon/registration_preview.html
+-rw-r--r--   0        0        0      438 2022-06-19 21:02:37.435258 leprikon-3.5.4/leprikon/templates/leprikon/registration_received/subject.html
+-rw-r--r--   0        0        0      165 2021-06-01 02:09:02.932873 leprikon-3.5.4/leprikon/templates/leprikon/registration_received/subject.subject.txt
+-rw-r--r--   0        0        0      433 2022-06-19 21:02:37.435258 leprikon-3.5.4/leprikon/templates/leprikon/registration_received/subject.txt
+-rw-r--r--   0        0        0     1031 2021-06-01 05:24:24.368881 leprikon-3.5.4/leprikon/templates/leprikon/registration_recipe.rml
+-rw-r--r--   0        0        0      712 2021-06-08 21:18:56.417557 leprikon-3.5.4/leprikon/templates/leprikon/registration_refund_offer/subject.html
+-rw-r--r--   0        0        0      180 2021-06-08 20:34:42.425099 leprikon-3.5.4/leprikon/templates/leprikon/registration_refund_offer/subject.subject.txt
+-rw-r--r--   0        0        0      575 2021-06-08 21:18:56.417557 leprikon-3.5.4/leprikon/templates/leprikon/registration_refund_offer/subject.txt
+-rw-r--r--   0        0        0      152 2021-02-06 20:07:28.154856 leprikon-3.5.4/leprikon/templates/leprikon/registration_refused/subject.html
+-rw-r--r--   0        0        0      177 2021-06-01 02:09:02.932873 leprikon-3.5.4/leprikon/templates/leprikon/registration_refused/subject.subject.txt
+-rw-r--r--   0        0        0      160 2021-02-06 20:07:28.154856 leprikon-3.5.4/leprikon/templates/leprikon/registration_refused/subject.txt
+-rw-r--r--   0        0        0      873 2021-02-06 20:07:28.154856 leprikon-3.5.4/leprikon/templates/leprikon/registrations.html
+-rw-r--r--   0        0        0     2387 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/reports/course_payments.html
+-rw-r--r--   0        0        0     4667 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/reports/course_payments_status.html
+-rw-r--r--   0        0        0     2263 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/reports/course_stats.html
+-rw-r--r--   0        0        0     1513 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/reports/debtors.html
+-rw-r--r--   0        0        0     2385 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/reports/event_payments.html
+-rw-r--r--   0        0        0     4656 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/reports/event_payments_status.html
+-rw-r--r--   0        0        0     2127 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/reports/event_stats.html
+-rw-r--r--   0        0        0     1934 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/reports/index.html
+-rw-r--r--   0        0        0     2405 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/reports/orderable_payments.html
+-rw-r--r--   0        0        0     4718 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/reports/orderable_payments_status.html
+-rw-r--r--   0        0        0     2151 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/reports/orderable_stats.html
+-rw-r--r--   0        0        0     2945 2021-06-01 08:37:09.566968 leprikon-3.5.4/leprikon/templates/leprikon/returned_payment_pdf/recipe.rml
+-rw-r--r--   0        0        0     2486 2021-05-31 10:12:28.917535 leprikon-3.5.4/leprikon/templates/leprikon/returned_payment_pdf/subject.rml
+-rw-r--r--   0        0        0      136 2021-05-31 12:22:27.052070 leprikon-3.5.4/leprikon/templates/leprikon/returned_payment_received/subject.html
+-rw-r--r--   0        0        0      223 2021-06-01 02:09:02.932873 leprikon-3.5.4/leprikon/templates/leprikon/returned_payment_received/subject.subject.txt
+-rw-r--r--   0        0        0      145 2021-05-31 12:22:27.052070 leprikon-3.5.4/leprikon/templates/leprikon/returned_payment_received/subject.txt
+-rw-r--r--   0        0        0      664 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/schoolyear_form.html
+-rw-r--r--   0        0        0       65 2021-02-06 20:07:28.158856 leprikon-3.5.4/leprikon/templates/leprikon/search.txt
+-rw-r--r--   0        0        0      765 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/static/bootstrap-datetimepicker.html
+-rw-r--r--   0        0        0      286 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/static/bootstrap-multiselect.html
+-rw-r--r--   0        0        0      273 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/static/ekko-lightbox.html
+-rw-r--r--   0        0        0       35 2021-02-06 20:07:28.158856 leprikon-3.5.4/leprikon/templates/leprikon/subject_form.html
+-rw-r--r--   0        0        0       72 2021-08-16 07:31:28.779948 leprikon-3.5.4/leprikon/templates/leprikon/subject_journals.html
+-rw-r--r--   0        0        0     1370 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/subject_list.html
+-rw-r--r--   0        0        0     4893 2022-09-11 14:45:14.421101 leprikon-3.5.4/leprikon/templates/leprikon/subject_preview.html
+-rw-r--r--   0        0        0    28074 2023-07-30 15:02:55.336964 leprikon-3.5.4/leprikon/templates/leprikon/subject_registration_form.html
+-rw-r--r--   0        0        0     3542 2021-06-03 02:51:13.941010 leprikon-3.5.4/leprikon/templates/leprikon/summary.html
+-rw-r--r--   0        0        0      235 2021-02-06 20:07:28.162856 leprikon-3.5.4/leprikon/templates/leprikon/terms_conditions.html
+-rw-r--r--   0        0        0     1959 2021-02-06 20:07:28.162856 leprikon-3.5.4/leprikon/templates/leprikon/timesheet_detail.html
+-rw-r--r--   0        0        0      898 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/timesheet_preview.html
+-rw-r--r--   0        0        0      189 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/templates/leprikon/timesheetentry_form.html
+-rw-r--r--   0        0        0        0 2021-02-06 20:07:28.162856 leprikon-3.5.4/leprikon/templates/leprikon/title.txt
+-rw-r--r--   0        0        0      134 2021-02-06 20:07:28.162856 leprikon-3.5.4/leprikon/templates/leprikon/user_create_form_item.html
+-rw-r--r--   0        0        0      572 2021-02-06 20:07:28.162856 leprikon-3.5.4/leprikon/templates/leprikon/user_dropdown.html
+-rw-r--r--   0        0        0      242 2021-02-06 20:07:28.162856 leprikon-3.5.4/leprikon/templates/leprikon/user_form.html
+-rw-r--r--   0        0        0      813 2021-02-06 20:07:28.162856 leprikon-3.5.4/leprikon/templates/leprikon/user_menu.html
+-rw-r--r--   0        0        0      283 2021-02-06 20:07:28.162856 leprikon-3.5.4/leprikon/templates/leprikon/widgets/input_option.html
+-rw-r--r--   0        0        0      211 2021-02-06 20:07:28.162856 leprikon-3.5.4/leprikon/templates/leprikon/widgets/multiple_input.html
+-rw-r--r--   0        0        0      554 2022-06-19 21:02:37.439258 leprikon-3.5.4/leprikon/templates/required_optional_field.html
+-rw-r--r--   0        0        0        0 2021-02-06 20:07:28.166856 leprikon-3.5.4/leprikon/templatetags/__init__.py
+-rw-r--r--   0        0        0     7364 2023-07-30 15:02:55.336964 leprikon-3.5.4/leprikon/templatetags/leprikon_tags.py
+-rw-r--r--   0        0        0      105 2023-01-01 16:24:39.600383 leprikon-3.5.4/leprikon/templatetags/staticfiles.py
+-rw-r--r--   0        0        0     5863 2023-07-30 15:02:55.340964 leprikon-3.5.4/leprikon/urls.py
+-rw-r--r--   0        0        0     9220 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/utils.py
+-rw-r--r--   0        0        0     7516 2021-08-16 07:31:28.779948 leprikon-3.5.4/leprikon/views/__init__.py
+-rw-r--r--   0        0        0     1659 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/views/billing_info.py
+-rw-r--r--   0        0        0      568 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/views/donation.py
+-rw-r--r--   0        0        0     5275 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/views/generic.py
+-rw-r--r--   0        0        0     5846 2023-01-09 01:29:07.000459 leprikon-3.5.4/leprikon/views/journals.py
+-rw-r--r--   0        0        0      706 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/views/leaders.py
+-rw-r--r--   0        0        0     1082 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/views/messages.py
+-rw-r--r--   0        0        0     1845 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/views/parents.py
+-rw-r--r--   0        0        0     2443 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/views/participants.py
+-rw-r--r--   0        0        0     2776 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/views/refundrequest.py
+-rw-r--r--   0        0        0     2150 2023-07-30 15:02:55.340964 leprikon-3.5.4/leprikon/views/registrationlink.py
+-rw-r--r--   0        0        0     1076 2021-02-15 21:00:52.274425 leprikon-3.5.4/leprikon/views/registrations.py
+-rw-r--r--   0        0        0     3486 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/views/reports/__init__.py
+-rw-r--r--   0        0        0     9337 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/views/reports/courses.py
+-rw-r--r--   0        0        0     2140 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/views/reports/debtors.py
+-rw-r--r--   0        0        0     7857 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/views/reports/events.py
+-rw-r--r--   0        0        0     8022 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/views/reports/orderables.py
+-rw-r--r--   0        0        0      628 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/views/schoolyear.py
+-rw-r--r--   0        0        0    12992 2023-07-30 15:02:55.340964 leprikon-3.5.4/leprikon/views/subjects.py
+-rw-r--r--   0        0        0     1845 2021-07-30 12:23:56.629387 leprikon-3.5.4/leprikon/views/summaries.py
+-rw-r--r--   0        0        0      130 2021-02-06 20:20:39.193125 leprikon-3.5.4/leprikon/views/terms_conditions.py
+-rw-r--r--   0        0        0     3175 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/views/timesheets.py
+-rw-r--r--   0        0        0     5378 2022-09-11 22:24:07.304086 leprikon-3.5.4/leprikon/views/user.py
+-rw-r--r--   0        0        0     2581 2023-08-07 14:41:23.641095 leprikon-3.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3271 1970-01-01 00:00:00.000000 leprikon-3.5.4/PKG-INFO
```

### Comparing `leprikon-3.5.3/LICENSE` & `leprikon-3.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/README.rst` & `leprikon-3.5.4/README.rst`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/__init__.py` & `leprikon-3.5.4/leprikon/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.5.3"
+__version__ = "3.5.4"
 default_app_config = "leprikon.apps.LeprikonConfig"
 
 staticfiles_urls = {
     "leprikon/lib/bootstrap/css/bootstrap-theme.css": "https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/css/bootstrap-theme.css",  # NOQA
     "leprikon/lib/bootstrap/css/bootstrap.min.css": "https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/css/bootstrap.min.css",  # NOQA
     "leprikon/lib/bootstrap/css/bootstrap-theme.css.map": "https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/css/bootstrap-theme.css.map",  # NOQA
     "leprikon/lib/bootstrap/css/bootstrap.min.css.map": "https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/css/bootstrap.min.css.map",  # NOQA
```

### Comparing `leprikon-3.5.3/leprikon/admin/__init__.py` & `leprikon-3.5.4/leprikon/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/agreements.py` & `leprikon-3.5.4/leprikon/admin/agreements.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/bulkupdate.py` & `leprikon-3.5.4/leprikon/admin/bulkupdate.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/courses.py` & `leprikon-3.5.4/leprikon/admin/courses.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/donation.py` & `leprikon-3.5.4/leprikon/admin/donation.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/events.py` & `leprikon-3.5.4/leprikon/admin/events.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/export.py` & `leprikon-3.5.4/leprikon/admin/export.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/filters.py` & `leprikon-3.5.4/leprikon/admin/filters.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/journals.py` & `leprikon-3.5.4/leprikon/admin/journals.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/leprikonsite.py` & `leprikon-3.5.4/leprikon/admin/leprikonsite.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/messages.py` & `leprikon-3.5.4/leprikon/admin/messages.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/orderables.py` & `leprikon-3.5.4/leprikon/admin/orderables.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/pdf.py` & `leprikon-3.5.4/leprikon/admin/pdf.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/refundrequest.py` & `leprikon-3.5.4/leprikon/admin/refundrequest.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/registrationlink.py` & `leprikon-3.5.4/leprikon/admin/registrationlink.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/roles.py` & `leprikon-3.5.4/leprikon/admin/roles.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/schoolyear.py` & `leprikon-3.5.4/leprikon/admin/schoolyear.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/subjects.py` & `leprikon-3.5.4/leprikon/admin/subjects.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/timesheets.py` & `leprikon-3.5.4/leprikon/admin/timesheets.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/transaction.py` & `leprikon-3.5.4/leprikon/admin/transaction.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/user.py` & `leprikon-3.5.4/leprikon/admin/user.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/admin/utils.py` & `leprikon-3.5.4/leprikon/admin/utils.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/api/serializers.py` & `leprikon-3.5.4/leprikon/api/serializers.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/api/urls.py` & `leprikon-3.5.4/leprikon/api/urls.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/api/views.py` & `leprikon-3.5.4/leprikon/api/views.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/apps.py` & `leprikon-3.5.4/leprikon/apps.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/bankreaders.py` & `leprikon-3.5.4/leprikon/bankreaders.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/cms_apps.py` & `leprikon-3.5.4/leprikon/cms_apps.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/cms_menus.py` & `leprikon-3.5.4/leprikon/cms_menus.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/cms_plugins/courses.py` & `leprikon-3.5.4/leprikon/cms_plugins/courses.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/cms_plugins/events.py` & `leprikon-3.5.4/leprikon/cms_plugins/events.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/cms_plugins/leaders.py` & `leprikon-3.5.4/leprikon/cms_plugins/leaders.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/cms_plugins/orderables.py` & `leprikon-3.5.4/leprikon/cms_plugins/orderables.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/cms_toolbars.py` & `leprikon-3.5.4/leprikon/cms_toolbars.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/conf/default_settings.py` & `leprikon-3.5.4/leprikon/conf/default_settings.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/cronjobs.py` & `leprikon-3.5.4/leprikon/cronjobs.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/forms/courses.py` & `leprikon-3.5.4/leprikon/forms/courses.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/forms/fields.py` & `leprikon-3.5.4/leprikon/forms/fields.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/forms/form.py` & `leprikon-3.5.4/leprikon/forms/form.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/forms/journals.py` & `leprikon-3.5.4/leprikon/forms/journals.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/forms/leaders.py` & `leprikon-3.5.4/leprikon/forms/leaders.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/forms/messages.py` & `leprikon-3.5.4/leprikon/forms/messages.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/forms/participant.py` & `leprikon-3.5.4/leprikon/forms/participant.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/forms/refundrequest.py` & `leprikon-3.5.4/leprikon/forms/refundrequest.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/forms/reports/courses.py` & `leprikon-3.5.4/leprikon/forms/reports/courses.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/forms/reports/events.py` & `leprikon-3.5.4/leprikon/forms/reports/events.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/forms/reports/orderables.py` & `leprikon-3.5.4/leprikon/forms/reports/orderables.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/forms/schoolyear.py` & `leprikon-3.5.4/leprikon/forms/schoolyear.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/forms/subjects.py` & `leprikon-3.5.4/leprikon/forms/subjects.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/forms/timesheets.py` & `leprikon-3.5.4/leprikon/forms/timesheets.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/forms/user.py` & `leprikon-3.5.4/leprikon/forms/user.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/forms/widgets.py` & `leprikon-3.5.4/leprikon/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/locale/cs/LC_MESSAGES/django.mo` & `leprikon-3.5.4/leprikon/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/locale/cs/LC_MESSAGES/django.po` & `leprikon-3.5.4/leprikon/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/locale/en/LC_MESSAGES/django.po` & `leprikon-3.5.4/leprikon/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/middleware.py` & `leprikon-3.5.4/leprikon/middleware.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0001_initial.py` & `leprikon-3.5.4/leprikon/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0002_initial_data.py` & `leprikon-3.5.4/leprikon/migrations/0002_initial_data.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0003_managers.py` & `leprikon-3.5.4/leprikon/migrations/0003_managers.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0005_subjectregistration_variable_symbol.py` & `leprikon-3.5.4/leprikon/migrations/0005_subjectregistration_variable_symbol.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0006_discount_periods.py` & `leprikon-3.5.4/leprikon/migrations/0006_discount_periods.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0007_bill_print_setup.py` & `leprikon-3.5.4/leprikon/migrations/0007_bill_print_setup.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0009_subjectpayment_received_by.py` & `leprikon-3.5.4/leprikon/migrations/0009_subjectpayment_received_by.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0012_subject_variants.py` & `leprikon-3.5.4/leprikon/migrations/0012_subject_variants.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0013_drop_insurance.py` & `leprikon-3.5.4/leprikon/migrations/0013_drop_insurance.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0015_school_year_divisions.py` & `leprikon-3.5.4/leprikon/migrations/0015_school_year_divisions.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0016_school_year_divisions_cleanup.py` & `leprikon-3.5.4/leprikon/migrations/0016_school_year_divisions_cleanup.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0017_citizenship.py` & `leprikon-3.5.4/leprikon/migrations/0017_citizenship.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0019_department.py` & `leprikon-3.5.4/leprikon/migrations/0019_department.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0020_agreements.py` & `leprikon-3.5.4/leprikon/migrations/0020_agreements.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0021_user_agreement.py` & `leprikon-3.5.4/leprikon/migrations/0021_user_agreement.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0022_bankreader.py` & `leprikon-3.5.4/leprikon/migrations/0022_bankreader.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0023_accountclosure.py` & `leprikon-3.5.4/leprikon/migrations/0023_accountclosure.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0025_agreements.py` & `leprikon-3.5.4/leprikon/migrations/0025_agreements.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0026_online_payments.py` & `leprikon-3.5.4/leprikon/migrations/0026_online_payments.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0027_journals.py` & `leprikon-3.5.4/leprikon/migrations/0027_journals.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0028_agegroups.py` & `leprikon-3.5.4/leprikon/migrations/0028_agegroups.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0029_payment_restrictions.py` & `leprikon-3.5.4/leprikon/migrations/0029_payment_restrictions.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0030_agreements.py` & `leprikon-3.5.4/leprikon/migrations/0030_agreements.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0031_registration_questions_agreements.py` & `leprikon-3.5.4/leprikon/migrations/0031_registration_questions_agreements.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0032_registration_participants_groups.py` & `leprikon-3.5.4/leprikon/migrations/0032_registration_participants_groups.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0033_target_groups.py` & `leprikon-3.5.4/leprikon/migrations/0033_target_groups.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0034_subject_registration_group.py` & `leprikon-3.5.4/leprikon/migrations/0034_subject_registration_group.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0035_on_delete.py` & `leprikon-3.5.4/leprikon/migrations/0035_on_delete.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0036_participants_instructed.py` & `leprikon-3.5.4/leprikon/migrations/0036_participants_instructed.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0037_message_sender.py` & `leprikon-3.5.4/leprikon/migrations/0037_message_sender.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0038_organizations.py` & `leprikon-3.5.4/leprikon/migrations/0038_organizations.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0039_editable_texts.py` & `leprikon-3.5.4/leprikon/migrations/0039_editable_texts.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0040_due_dates.py` & `leprikon-3.5.4/leprikon/migrations/0040_due_dates.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0041_billing_info.py` & `leprikon-3.5.4/leprikon/migrations/0041_billing_info.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0042_chat_group_types.py` & `leprikon-3.5.4/leprikon/migrations/0042_chat_group_types.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0043_registration_links.py` & `leprikon-3.5.4/leprikon/migrations/0043_registration_links.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0044_billinginfo_contacts.py` & `leprikon-3.5.4/leprikon/migrations/0044_billinginfo_contacts.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0045_registration_slug.py` & `leprikon-3.5.4/leprikon/migrations/0045_registration_slug.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0046_attachment_events.py` & `leprikon-3.5.4/leprikon/migrations/0046_attachment_events.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0047_pr_print_setup.py` & `leprikon-3.5.4/leprikon/migrations/0047_pr_print_setup.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0048_birth_date.py` & `leprikon-3.5.4/leprikon/migrations/0048_birth_date.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0049_target_groups_fix.py` & `leprikon-3.5.4/leprikon/migrations/0049_target_groups_fix.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0050_orderables.py` & `leprikon-3.5.4/leprikon/migrations/0050_orderables.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0051_registration_group_name.py` & `leprikon-3.5.4/leprikon/migrations/0051_registration_group_name.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0052_payment_notification_sent.py` & `leprikon-3.5.4/leprikon/migrations/0052_payment_notification_sent.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0053_registration_dates_by.py` & `leprikon-3.5.4/leprikon/migrations/0053_registration_dates_by.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0055_schoolyearblockplugin.py` & `leprikon-3.5.4/leprikon/migrations/0055_schoolyearblockplugin.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0056_registration_period.py` & `leprikon-3.5.4/leprikon/migrations/0056_registration_period.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0057_registration_period.py` & `leprikon-3.5.4/leprikon/migrations/0057_registration_period.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0058_agegroup_min_max_age.py` & `leprikon-3.5.4/leprikon/migrations/0058_agegroup_min_max_age.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0059_transactions_data.py` & `leprikon-3.5.4/leprikon/migrations/0059_transactions_data.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0060_transactions.py` & `leprikon-3.5.4/leprikon/migrations/0060_transactions.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0061_refundrequest.py` & `leprikon-3.5.4/leprikon/migrations/0061_refundrequest.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0062_refund_offers.py` & `leprikon-3.5.4/leprikon/migrations/0062_refund_offers.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0063_journals.py` & `leprikon-3.5.4/leprikon/migrations/0063_journals.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0064_journals_cleanup.py` & `leprikon-3.5.4/leprikon/migrations/0064_journals_cleanup.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0065_subject_type_page.py` & `leprikon-3.5.4/leprikon/migrations/0065_subject_type_page.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0067_remove_rocketchat.py` & `leprikon-3.5.4/leprikon/migrations/0067_remove_rocketchat.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0068_participant_answers.py` & `leprikon-3.5.4/leprikon/migrations/0068_participant_answers.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0069_question_slug.py` & `leprikon-3.5.4/leprikon/migrations/0069_question_slug.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0070_decision_print_setup.py` & `leprikon-3.5.4/leprikon/migrations/0070_decision_print_setup.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0071_transaction_amount.py` & `leprikon-3.5.4/leprikon/migrations/0071_transaction_amount.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0072_prices.py` & `leprikon-3.5.4/leprikon/migrations/0072_prices.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0073_add_limit_choices_to.py` & `leprikon-3.5.4/leprikon/migrations/0073_add_limit_choices_to.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0074_schoolyear_period_order.py` & `leprikon-3.5.4/leprikon/migrations/0074_schoolyear_period_order.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0075_journal_school_year_division.py` & `leprikon-3.5.4/leprikon/migrations/0075_journal_school_year_division.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0076_journalentry_period.py` & `leprikon-3.5.4/leprikon/migrations/0076_journalentry_period.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0078_delete_coursevariant.py` & `leprikon-3.5.4/leprikon/migrations/0078_delete_coursevariant.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/migrations/0079_mandatory_subject_variants.py` & `leprikon-3.5.4/leprikon/migrations/0079_mandatory_subject_variants.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/account.py` & `leprikon-3.5.4/leprikon/models/account.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/agegroup.py` & `leprikon-3.5.4/leprikon/models/agegroup.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/agreements.py` & `leprikon-3.5.4/leprikon/models/agreements.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/citizenship.py` & `leprikon-3.5.4/leprikon/models/citizenship.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/courses.py` & `leprikon-3.5.4/leprikon/models/courses.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/department.py` & `leprikon-3.5.4/leprikon/models/department.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/donation.py` & `leprikon-3.5.4/leprikon/models/donation.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/events.py` & `leprikon-3.5.4/leprikon/models/events.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/fields.py` & `leprikon-3.5.4/leprikon/models/fields.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/journals.py` & `leprikon-3.5.4/leprikon/models/journals.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/leprikonsite.py` & `leprikon-3.5.4/leprikon/models/leprikonsite.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/messages.py` & `leprikon-3.5.4/leprikon/models/messages.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/orderables.py` & `leprikon-3.5.4/leprikon/models/orderables.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/organizations.py` & `leprikon-3.5.4/leprikon/models/organizations.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/pdfmail.py` & `leprikon-3.5.4/leprikon/models/pdfmail.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/place.py` & `leprikon-3.5.4/leprikon/models/place.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/printsetup.py` & `leprikon-3.5.4/leprikon/models/printsetup.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/question.py` & `leprikon-3.5.4/leprikon/models/question.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/refundrequest.py` & `leprikon-3.5.4/leprikon/models/refundrequest.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/registrationlink.py` & `leprikon-3.5.4/leprikon/models/registrationlink.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/roles.py` & `leprikon-3.5.4/leprikon/models/roles.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/school.py` & `leprikon-3.5.4/leprikon/models/school.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/schoolyear.py` & `leprikon-3.5.4/leprikon/models/schoolyear.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/startend.py` & `leprikon-3.5.4/leprikon/models/startend.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/subjects.py` & `leprikon-3.5.4/leprikon/models/subjects.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/targetgroup.py` & `leprikon-3.5.4/leprikon/models/targetgroup.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/test_utils.py` & `leprikon-3.5.4/leprikon/models/test_utils.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/times.py` & `leprikon-3.5.4/leprikon/models/times.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/timesheets.py` & `leprikon-3.5.4/leprikon/models/timesheets.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/transaction.py` & `leprikon-3.5.4/leprikon/models/transaction.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/models/utils.py` & `leprikon-3.5.4/leprikon/models/utils.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/search_indexes/base.py` & `leprikon-3.5.4/leprikon/search_indexes/base.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/site/settings.py` & `leprikon-3.5.4/leprikon/site/settings.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/site/urls.py` & `leprikon-3.5.4/leprikon/site/urls.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/static/admin/css/scrollbars.css` & `leprikon-3.5.4/leprikon/static/admin/css/scrollbars.css`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/static/admin/js/admin/RelatedObjectLookups.js` & `leprikon-3.5.4/leprikon/static/admin/js/admin/RelatedObjectLookups.js`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/static/favicon.ico` & `leprikon-3.5.4/leprikon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/static/leprikon/css/colors.css` & `leprikon-3.5.4/leprikon/static/leprikon/css/colors.css`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/static/leprikon/css/layout.css` & `leprikon-3.5.4/leprikon/static/leprikon/css/layout.css`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/static/leprikon/css/registrations.changelist.css` & `leprikon-3.5.4/leprikon/static/leprikon/css/registrations.changelist.css`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/static/leprikon/fonts/DejaVuSans-Bold.ttf` & `leprikon-3.5.4/leprikon/static/leprikon/fonts/DejaVuSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/static/leprikon/fonts/DejaVuSans-BoldOblique.ttf` & `leprikon-3.5.4/leprikon/static/leprikon/fonts/DejaVuSans-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/static/leprikon/fonts/DejaVuSans-Oblique.ttf` & `leprikon-3.5.4/leprikon/static/leprikon/fonts/DejaVuSans-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/static/leprikon/fonts/DejaVuSans.ttf` & `leprikon-3.5.4/leprikon/static/leprikon/fonts/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/static/leprikon/img/leprikon-kuk-l.png` & `leprikon-3.5.4/leprikon/static/leprikon/img/leprikon-kuk-l.png`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/static/leprikon/img/logo-horizontal.png` & `leprikon-3.5.4/leprikon/static/leprikon/img/logo-horizontal.png`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/static/leprikon/img/logo.png` & `leprikon-3.5.4/leprikon/static/leprikon/img/logo.png`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/static/leprikon/js/Popup.js` & `leprikon-3.5.4/leprikon/static/leprikon/js/Popup.js`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/static/leprikon/js/required_optional_field.js` & `leprikon-3.5.4/leprikon/static/leprikon/js/required_optional_field.js`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/admin/base.html` & `leprikon-3.5.4/leprikon/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/admin/change_list.html` & `leprikon-3.5.4/leprikon/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/admin/change_list_results.html` & `leprikon-3.5.4/leprikon/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/admin/inc/branding.html` & `leprikon-3.5.4/leprikon/templates/admin/inc/branding.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/admin/leprikon/donation/change_form.html` & `leprikon-3.5.4/leprikon/templates/admin/leprikon/donation/change_form.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/admin/leprikon/message/add_recipients.html` & `leprikon-3.5.4/leprikon/templates/admin/leprikon/message/add_recipients.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/admin/leprikon/messagerecipient/send_mails.html` & `leprikon-3.5.4/leprikon/templates/admin/leprikon/messagerecipient/send_mails.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/admin/leprikon/subjectreceivedpayment/change_form.html` & `leprikon-3.5.4/leprikon/templates/admin/leprikon/subjectreceivedpayment/change_form.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/admin/leprikon/subjectreturnedpayment/change_form.html` & `leprikon-3.5.4/leprikon/templates/admin/leprikon/subjectreturnedpayment/change_form.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/admin/action_form.html` & `leprikon-3.5.4/leprikon/templates/leprikon/admin/action_form.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/admin/bulk_update_form.html` & `leprikon-3.5.4/leprikon/templates/leprikon/admin/bulk_update_form.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/admin/dashboard.html` & `leprikon-3.5.4/leprikon/templates/leprikon/admin/dashboard.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/admin/merge.html` & `leprikon-3.5.4/leprikon/templates/leprikon/admin/merge.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/admin/send_message.html` & `leprikon-3.5.4/leprikon/templates/leprikon/admin/send_message.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/alternating.html` & `leprikon-3.5.4/leprikon/templates/leprikon/alternating.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/base.html` & `leprikon-3.5.4/leprikon/templates/leprikon/base.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/billing_info_preview.html` & `leprikon-3.5.4/leprikon/templates/leprikon/billing_info_preview.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/cms/course_list_filtered.html` & `leprikon-3.5.4/leprikon/templates/leprikon/cms/course_list_filtered.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/cms/event_list_filtered.html` & `leprikon-3.5.4/leprikon/templates/leprikon/cms/event_list_filtered.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/cms/leader_list/default.html` & `leprikon-3.5.4/leprikon/templates/leprikon/cms/leader_list/default.html`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         {% if leader.all_public_contacts %}
         <p>
             {% trans 'Contact' %}:<br/>
             <ul class="contacts">
             {% for contact in leader.all_public_contacts %}
                 <li class="contact contact-{{ contact.contact_type }}">
                     {{ contact.contact }}
-                </div>
+                </li>
             {% endfor %}
             </ul>
         </p>
         {% endif %}
 
         {% if leader.page %}
         <p>
```

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/cms/leader_list_filtered.html` & `leprikon-3.5.4/leprikon/templates/leprikon/cms/leader_list_filtered.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/cms/orderable_list_filtered.html` & `leprikon-3.5.4/leprikon/templates/leprikon/cms/orderable_list_filtered.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/confirm_form.html` & `leprikon-3.5.4/leprikon/templates/leprikon/confirm_form.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/course_registrations.html` & `leprikon-3.5.4/leprikon/templates/leprikon/course_registrations.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/donation_pdf/default.rml` & `leprikon-3.5.4/leprikon/templates/leprikon/donation_pdf/default.rml`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/donation_pdf/recipe.rml` & `leprikon-3.5.4/leprikon/templates/leprikon/donation_pdf/recipe.rml`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/donations.html` & `leprikon-3.5.4/leprikon/templates/leprikon/donations.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/event_registrations.html` & `leprikon-3.5.4/leprikon/templates/leprikon/event_registrations.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/filter_form.html` & `leprikon-3.5.4/leprikon/templates/leprikon/filter_form.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/filtered_subject_list.html` & `leprikon-3.5.4/leprikon/templates/leprikon/filtered_subject_list.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/form.html` & `leprikon-3.5.4/leprikon/templates/leprikon/form.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/form_item_checkbox.html` & `leprikon-3.5.4/leprikon/templates/leprikon/form_item_checkbox.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/invoices.xml` & `leprikon-3.5.4/leprikon/templates/leprikon/invoices.xml`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/journal_form.html` & `leprikon-3.5.4/leprikon/templates/leprikon/journal_form.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/journal_journal.html` & `leprikon-3.5.4/leprikon/templates/leprikon/journal_journal.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/journal_journal_pdf/default.rml` & `leprikon-3.5.4/leprikon/templates/leprikon/journal_journal_pdf/default.rml`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/journal_preview.html` & `leprikon-3.5.4/leprikon/templates/leprikon/journal_preview.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/journalentry_form.html` & `leprikon-3.5.4/leprikon/templates/leprikon/journalentry_form.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/leader_list.html` & `leprikon-3.5.4/leprikon/templates/leprikon/leader_list.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/leader_preview.html` & `leprikon-3.5.4/leprikon/templates/leprikon/leader_preview.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/leader_summary.html` & `leprikon-3.5.4/leprikon/templates/leprikon/leader_summary.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/list.html` & `leprikon-3.5.4/leprikon/templates/leprikon/list.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/login.html` & `leprikon-3.5.4/leprikon/templates/leprikon/login.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/menu.html` & `leprikon-3.5.4/leprikon/templates/leprikon/menu.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/messagerecipient_detail.html` & `leprikon-3.5.4/leprikon/templates/leprikon/messagerecipient_detail.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/messages_table.html` & `leprikon-3.5.4/leprikon/templates/leprikon/messages_table.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/modal_messages.html` & `leprikon-3.5.4/leprikon/templates/leprikon/modal_messages.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/orderable_registrations.html` & `leprikon-3.5.4/leprikon/templates/leprikon/orderable_registrations.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/pagination.html` & `leprikon-3.5.4/leprikon/templates/leprikon/pagination.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/parent_preview.html` & `leprikon-3.5.4/leprikon/templates/leprikon/parent_preview.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/participant_preview.html` & `leprikon-3.5.4/leprikon/templates/leprikon/participant_preview.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/password_reset_email.html` & `leprikon-3.5.4/leprikon/templates/leprikon/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/payments.html` & `leprikon-3.5.4/leprikon/templates/leprikon/payments.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/received_payment_pdf/recipe.rml` & `leprikon-3.5.4/leprikon/templates/leprikon/received_payment_pdf/recipe.rml`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/received_payment_pdf/subject.rml` & `leprikon-3.5.4/leprikon/templates/leprikon/received_payment_pdf/subject.rml`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/registration_decision/subject.rml` & `leprikon-3.5.4/leprikon/templates/leprikon/registration_decision/subject.rml`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/registration_details.html` & `leprikon-3.5.4/leprikon/templates/leprikon/registration_details.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/registration_links.html` & `leprikon-3.5.4/leprikon/templates/leprikon/registration_links.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/registration_mail_details.html` & `leprikon-3.5.4/leprikon/templates/leprikon/registration_mail_details.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/registration_mail_details.txt` & `leprikon-3.5.4/leprikon/templates/leprikon/registration_mail_details.txt`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/registration_payment_request/subject.html` & `leprikon-3.5.4/leprikon/templates/leprikon/registration_payment_request/subject.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/registration_payment_request/subject.rml` & `leprikon-3.5.4/leprikon/templates/leprikon/registration_payment_request/subject.rml`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/registration_payment_request/subject.txt` & `leprikon-3.5.4/leprikon/templates/leprikon/registration_payment_request/subject.txt`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/registration_payments.html` & `leprikon-3.5.4/leprikon/templates/leprikon/registration_payments.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/registration_pdf/subject.rml` & `leprikon-3.5.4/leprikon/templates/leprikon/registration_pdf/subject.rml`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/registration_preview.html` & `leprikon-3.5.4/leprikon/templates/leprikon/registration_preview.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/registration_recipe.rml` & `leprikon-3.5.4/leprikon/templates/leprikon/registration_recipe.rml`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/registration_refund_offer/subject.html` & `leprikon-3.5.4/leprikon/templates/leprikon/registration_refund_offer/subject.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/registration_refund_offer/subject.txt` & `leprikon-3.5.4/leprikon/templates/leprikon/registration_refund_offer/subject.txt`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/registrations.html` & `leprikon-3.5.4/leprikon/templates/leprikon/registrations.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/reports/course_payments.html` & `leprikon-3.5.4/leprikon/templates/leprikon/reports/course_payments.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/reports/course_payments_status.html` & `leprikon-3.5.4/leprikon/templates/leprikon/reports/course_payments_status.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/reports/course_stats.html` & `leprikon-3.5.4/leprikon/templates/leprikon/reports/course_stats.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/reports/debtors.html` & `leprikon-3.5.4/leprikon/templates/leprikon/reports/debtors.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/reports/event_payments.html` & `leprikon-3.5.4/leprikon/templates/leprikon/reports/event_payments.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/reports/event_payments_status.html` & `leprikon-3.5.4/leprikon/templates/leprikon/reports/event_payments_status.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/reports/event_stats.html` & `leprikon-3.5.4/leprikon/templates/leprikon/reports/event_stats.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/reports/index.html` & `leprikon-3.5.4/leprikon/templates/leprikon/reports/index.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/reports/orderable_payments.html` & `leprikon-3.5.4/leprikon/templates/leprikon/reports/orderable_payments.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/reports/orderable_payments_status.html` & `leprikon-3.5.4/leprikon/templates/leprikon/reports/orderable_payments_status.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/reports/orderable_stats.html` & `leprikon-3.5.4/leprikon/templates/leprikon/reports/orderable_stats.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/returned_payment_pdf/recipe.rml` & `leprikon-3.5.4/leprikon/templates/leprikon/returned_payment_pdf/recipe.rml`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/returned_payment_pdf/subject.rml` & `leprikon-3.5.4/leprikon/templates/leprikon/returned_payment_pdf/subject.rml`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/schoolyear_form.html` & `leprikon-3.5.4/leprikon/templates/leprikon/schoolyear_form.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/static/bootstrap-datetimepicker.html` & `leprikon-3.5.4/leprikon/templates/leprikon/static/bootstrap-datetimepicker.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/subject_list.html` & `leprikon-3.5.4/leprikon/templates/leprikon/subject_list.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/subject_preview.html` & `leprikon-3.5.4/leprikon/templates/leprikon/subject_preview.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/subject_registration_form.html` & `leprikon-3.5.4/leprikon/templates/leprikon/subject_registration_form.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/summary.html` & `leprikon-3.5.4/leprikon/templates/leprikon/summary.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/timesheet_detail.html` & `leprikon-3.5.4/leprikon/templates/leprikon/timesheet_detail.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/timesheet_preview.html` & `leprikon-3.5.4/leprikon/templates/leprikon/timesheet_preview.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/user_dropdown.html` & `leprikon-3.5.4/leprikon/templates/leprikon/user_dropdown.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/leprikon/user_menu.html` & `leprikon-3.5.4/leprikon/templates/leprikon/user_menu.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templates/required_optional_field.html` & `leprikon-3.5.4/leprikon/templates/required_optional_field.html`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/templatetags/leprikon_tags.py` & `leprikon-3.5.4/leprikon/templatetags/leprikon_tags.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/urls.py` & `leprikon-3.5.4/leprikon/urls.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/utils.py` & `leprikon-3.5.4/leprikon/utils.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/__init__.py` & `leprikon-3.5.4/leprikon/views/__init__.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/billing_info.py` & `leprikon-3.5.4/leprikon/views/billing_info.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/donation.py` & `leprikon-3.5.4/leprikon/views/donation.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/generic.py` & `leprikon-3.5.4/leprikon/views/generic.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/journals.py` & `leprikon-3.5.4/leprikon/views/journals.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/leaders.py` & `leprikon-3.5.4/leprikon/views/leaders.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/messages.py` & `leprikon-3.5.4/leprikon/views/messages.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/parents.py` & `leprikon-3.5.4/leprikon/views/parents.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/participants.py` & `leprikon-3.5.4/leprikon/views/participants.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/refundrequest.py` & `leprikon-3.5.4/leprikon/views/refundrequest.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/registrationlink.py` & `leprikon-3.5.4/leprikon/views/registrationlink.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/registrations.py` & `leprikon-3.5.4/leprikon/views/registrations.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/reports/__init__.py` & `leprikon-3.5.4/leprikon/views/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/reports/courses.py` & `leprikon-3.5.4/leprikon/views/reports/courses.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/reports/debtors.py` & `leprikon-3.5.4/leprikon/views/reports/debtors.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/reports/events.py` & `leprikon-3.5.4/leprikon/views/reports/events.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/reports/orderables.py` & `leprikon-3.5.4/leprikon/views/reports/orderables.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/schoolyear.py` & `leprikon-3.5.4/leprikon/views/schoolyear.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/subjects.py` & `leprikon-3.5.4/leprikon/views/subjects.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/summaries.py` & `leprikon-3.5.4/leprikon/views/summaries.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/timesheets.py` & `leprikon-3.5.4/leprikon/views/timesheets.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/leprikon/views/user.py` & `leprikon-3.5.4/leprikon/views/user.py`

 * *Files identical despite different names*

### Comparing `leprikon-3.5.3/pyproject.toml` & `leprikon-3.5.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 known_first_party = "leprikon"
 line_length = 120
 profile = "black"
 skip_glob = "*migrations*"
 
 [tool.poetry]
 name = "leprikon"
-version = "3.5.3"
+version = "3.5.4"
 description = "Django CMS based IS for education"
 authors = ["Jakub Dorňák <jakub.dornak@misli.cz>"]
 license = "BSD-3-Clause"
 readme = "README.rst"
 homepage = "https://leprikon.cz/"
 repository = "https://github.com/leprikon-cz/leprikon"
 classifiers = [
```

### Comparing `leprikon-3.5.3/PKG-INFO` & `leprikon-3.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leprikon
-Version: 3.5.3
+Version: 3.5.4
 Summary: Django CMS based IS for education
 Home-page: https://leprikon.cz/
 License: BSD-3-Clause
 Author: Jakub Dorňák
 Author-email: jakub.dornak@misli.cz
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

