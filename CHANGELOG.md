# Change Log

All notable changes to this project will be documented in this file.

### 2.1.0 - 2020-07-05

### Added
- [20: Support for custom rate limit values](https://github.com/nikolaposa/rate-limit/pull/20)
- [25: APCu Rate Limiter](https://github.com/nikolaposa/rate-limit/pull/25)
- [26: Predis Rate Limiter](https://github.com/nikolaposa/rate-limit/pull/26)
- [28: Memcached Rate Limiter](https://github.com/nikolaposa/rate-limit/pull/28)
- [32: In-memory Rate Limiter](https://github.com/nikolaposa/rate-limit/pull/32)

## 2.0.0 - 2020-03-22

### Added
- `Rate` object representing "per unit of time" rate of operations

### Changed
- PHP 7.2 is now the minimum required version
- `RateLimiter` now accepts `identifier` and `Rate` so rate can be specified during runtime

### Removed
- `RateLimitMiddleware` (moved to a separate [rate-limit-middleware](https://github.com/nikolaposa/rate-limit-middleware) repository)

## 1.0.1 - 2017-10-25

### Fixed
- [6: Fix X-RateLimit-Remaining wave issue](https://github.com/nikolaposa/rate-limit/pull/6)

## 1.0.0 - 2017-02-14

## 0.4.0 - 2017-02-09

### Changed
- [4: Standalone rate limiter](https://github.com/nikolaposa/rate-limit/pull/4)

## 0.3.0 - 2017-02-04

### Added
- [3: Ability to whitelist requests](https://github.com/nikolaposa/rate-limit/pull/3)

### Changed
- Default identity is now generated based on certain request attributes
- Instead of returning default value, Storage raises exception if value doesn't exist under key

### Fixed
- Fixed Redis-backed rate limiter factory

## 0.2.0 - 2017-01-27

### Added
- [2: Redis-based storage](https://github.com/nikolaposa/rate-limit/pull/2)

### Changed
- [1: Atomic storage design](https://github.com/nikolaposa/rate-limit/pull/1)
- Rename `IdentityGenerator` to `IdentityResolver`


[link-unreleased]: https://github.com/nikolaposa/rate-limit/compare/2.0.0...HEAD
