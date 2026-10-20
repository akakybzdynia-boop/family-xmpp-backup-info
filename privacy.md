---
title: Privacy policy — Family XMPP Backup
---

# Privacy policy

Effective date: 20 October 2026.

## Purpose and Google Drive access

Family XMPP Backup is operated for personal use by the Google account owner.
It requests the Google Drive permission drive.file to create and manage backup
files created by this application. The permission is not intended to provide
access to unrelated files in the account.

Backup operations upload encrypted data, list and read backup objects, and
delete obsolete backup objects according to the configured retention policy.
Restore and integrity-check operations read encrypted backup objects.

## Storage and protection

Restic encrypts backup content and its file metadata on the source server before
uploading it to Google Drive. Google Drive still receives encrypted objects and
can observe service metadata such as object sizes and access times.

The OAuth refresh token is stored in a restricted configuration file on the
backup server. The restic password is stored separately from the remote
repository. Recovery copies of credentials must be kept in private storage
controlled by the operator.

## Use and disclosure

Data accessed through Google Drive is used only for backup, retention,
integrity checking and recovery. The operator does not sell this data, use it
for advertising, or disclose it to unrelated third parties.

Google processes stored objects and API traffic under its applicable terms.
GitHub hosts these public information pages and may process website request
metadata under its own privacy statement. These pages contain no analytics,
advertising or application sign-in form.

## Retention, revocation and deletion

Backup objects are retained according to the operator's backup policy and are
deleted as snapshots expire. The account owner can revoke the application's
access in Google Account settings. Revocation stops future access but does not
automatically delete files already stored in Google Drive.

The account owner can delete the application's backup folder through Google
Drive. Deleting a restic repository can make its backups irrecoverable.

## Contact and changes

This is a personal utility with no public registration. Questions about these
information pages can be raised through this repository's GitHub issue tracker.
Do not include credentials, messages or other private data in a public issue.

This policy will be updated if the application's data handling changes.
