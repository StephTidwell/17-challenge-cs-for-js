# Regex Tutorial - Matching a URL

## Summary

A regular expression is a pattern used to match character combinations in text. The regex for matching an email address consists of several parts: the local part, which appears before the @ symbol and can contain uppercase letters, digits, period, underscore, percent sign, plus sign, or hyphen; the @ symbol; the domain part, which appears after the @ symbol and can contain uppercase letters, digits, period, or hyphen; and the top-level domain, which appears after the last period and can contain two or more uppercase letters.

## Table of Contents

- [Introduction](#introduction)
- [Let's break it down](#lets-break-it-down)
- [Conclusion](#conclusion)

## Introduction

This regular expression should match most valid URLs that follow the `http`, `https`, or `ftp` protocols.

`^(https?|ftp):\/\/[^\s/$.?#].[^\s]*$`

## Let's break it down:

This regex uses the following elements:

`^` - This anchors the regex to the beginning of the string, ensuring that the match starts at the beginning of the URL.
`(https?|ftp)` - This is a group that matches either http, https, or ftp.
`:\/\/` - This matches the colon and two slashes that follow the protocol.
`[^\s/$.?#]` - This is a character set that matches any character that is not a whitespace, forward slash, question mark, period, or hash. It ensures that the domain name starts with a non-special character.
`.` - This matches the first character of the domain name after the protocol.
`[^\s]*` - This matches any number of non-whitespace characters that follow the first character of the domain name.
`$` - This anchors the regex to the end of the string, ensuring that the match ends at the end of the URL.

## Conclusion

This regular expression should match most valid URLs that follow the http, https, or ftp protocols. Note that this regex does not match URLs that contain query parameters or anchor tags. If you need to match those as well, you'll need to modify the regex accordingly.

I hope you found this tutorial helpful and please see below for my contact information.

## Author

**Author**: Stephanie Tidwell

**About me**: Current student at UNH Coding Bootcamp.

**Github**: [Link Here ](https://github.com/StephTidwell)

**Github Repo**: [Link Here ](https://github.com/StephTidwell/17-challenge-cs-for-js)

**Github Gist**: [Challenge 17 Link Here ](https://gist.github.com/StephTidwell/1c45bc547799f13eee6d7d00dc837b46)
