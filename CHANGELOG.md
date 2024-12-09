# Changelog

## [0.3.0] - 2024-03-XX

### Added

- Support for fetching rules from two repositories:
  - Official repo: `PatrickJS/awesome-cursorrules`
  - Custom repo: `juanma-ai/my-cursor-rules`
- Source indicator in QuickPick UI showing which repository each rule comes from
- Progress interface for better type safety
- Custom rules now appear first in the selection list
- Added context parameter to `fetchCursorRuleContent` for proper cache access

### Changed

- Updated dependencies and type definitions:
  - Updated @types/axios to ^0.14.4
  - Updated @types/node to ^22.10.1
  - Updated @types/vscode to ^1.95.0
- Modified `tsconfig.json` to include 'dom' lib for console support
- Improved code formatting with consistent double quotes
- Enhanced error handling for repository fetching
- Updated function signatures to properly pass extension context

### Fixed

- Fixed type errors in githubApi.ts and addCursorRule.ts
- Fixed linter errors related to missing type declarations
- Fixed console.error type definition by adding DOM lib
- Fixed progress parameter typing in withProgress calls
- Fixed context access in fetchCursorRuleContent function

### Technical Improvements

- Refactored `fetchCursorRulesList` to handle multiple repositories
- Added proper TypeScript types for Progress interface
- Improved error handling in repository fetching
- Enhanced caching mechanism to handle multiple sources
- Added source tracking for each rule
- Improved cache instance management with proper context handling

### Code Style

- Standardized string quotes to double quotes
- Improved code formatting and indentation
- Added proper type annotations
- Enhanced function signatures with explicit return types

### Development

- Added new type definitions for better development experience
- Updated TypeScript configuration for better type checking
- Improved development tooling with better type support