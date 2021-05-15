# Flutter intl package tools

Intl package is used to perform localization and internationalization of a flutter app.

1. To create arb files run the commands:
   `flutter pub run intl_translation:extract_to_arb --output-dir [path-to-dir]input-dart-files-with-strings`
   Example:
   `flutter pub run intl_translation:extract_to_arb --output-dir lib/shared/strings lib/shared/strings/app_strings.dart`

2. To generate intl_messages_all.dart file:
   `flutter pub run intl_translation:generate_from_arb --output-dir [path-to-dir] dart-file-with-class-strings path-to-arb-files`
   Example:
   `flutter pub run intl_translation:generate_from_arb --codegen_mode release --output-dir lib/shared/strings lib/shared/strings/app_strings.dart lib/shared/strings/intl_messages.arb`
