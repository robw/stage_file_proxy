Stage File Proxy saves you development time and disk space.

When developing Drupal sites locally, you often face a choice between broken
images and taking the time to copy a snapshot of the remote files directory,
which might be several gigabytes large, depending on the site. Stage File Proxy
lets you update the database of your local development instance without having
to update your files directory. Stage File Proxy transfers each requested file
just in time when it is requested. This is especially useful for large sites
with huge numbers of files. Stage File Proxy has an additional mode in which it
can serve a 301 redirect to files on the server, so it's possible to see all
your images without having a local files directory at all.

Stage File Proxy integrates with imagecache to transfer the original image from
the origin and then resize it locally.

This module is only tested using Apache 2 on Mac OS X and Linux. You should not
need to have this module enabled in production. It also assumes, for now, that
you have the same relative path (e.g. '/files' or /sites/default/files') on both
production and development environments.

http://drupal.org/project/stage_file_proxy

Original project by Austin Smith (http://drupal.org/user/199298).
Ported to D7 by Rob Wilmshurst (http://drupal.org/user/144488).
