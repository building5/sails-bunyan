# sails-bunyan changelog

## v1.0.6 (2015-09-29)

 * #4 Fix request logger injection.

## v1.0.5 (2015-06-12)

 * Manually serialize requests when building the child logger, since bunyan
   doesn't do that for us.

## v1.0.4 (2015-06-08)

 * Change request logger to build simple loggers, so that streams are shared
   between the parent and children. This solves some crashing problems when
   `.reopenFileStreams()` is called.

## v1.0.3 (2015-06-02)

 * Updated README to point to sails-hook-bunyan.

## v1.0.2 (2015-03-04)

 * #3 export logLevels, so sails-bunyan extensions can make their
   own mappings

## v1.0.1 (2015-01-06)

 * Doc updates
 * Fix level setting when using `config.filePath`.

## v1.0.0 (2014-11-06)

 * `config.filePath` for file logging
 * `config.rotationSignal` for file rotation
 * `config.logUncaughtException` to log uncaught exceptions with Bunyan
   and exit.

## v0.1.0 (2014-08-27)

 * Initial Release
