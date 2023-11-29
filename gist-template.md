#Regex-Tutorial

Regex-
Lets look at a simple regex pattern to try and understand what regex is

Regex Pattern: /^[a-zA-Z0-9._-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,4}$/

Explanation:

    / and /: Delimiters that indicate the start and end of the regex pattern.

    ^: Anchors the regex at the beginning of the string. It asserts the start of the line.

    [a-zA-Z0-9._-]+: Matches one or more of the characters inside the square brackets. In this case, it matches any combination of uppercase letters, lowercase letters, digits, periods (.), underscores (_), and hyphens (-).

    @: Matches the at symbol.

    [a-zA-Z0-9.-]+: Similar to the first character class, it matches one or more characters that can be uppercase letters, lowercase letters, digits, periods (.), or hyphens (-). This is used for the domain name before the dot.

    \.: Escapes the dot (.) since it has a special meaning in regex. Matches a literal dot.

    [a-zA-Z]{2,4}: Matches between 2 and 4 characters that can be uppercase or lowercase letters. This is used for the top-level domain (TLD) like com, net, org.

    $: Anchors the regex at the end of the string. It asserts the end of the line.