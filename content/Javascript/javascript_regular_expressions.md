/*
Title: JavaScript Regular Expressions
*/

[資料來源:w3schools](http://www.w3schools.com/js/js_regexp.asp)
### Syntax

```
/pattern/modifiers
```
<br>

### Regular Expression Modifiers

**Modifiers** can be used to perform case-insensitive more global searches:

<table>
	<tr>
		<th>Modifier</th>
		<th>Description</th>
	</tr>
    <tr>
        <td>i</td>
        <td>Perform case-insensitive matching</td>
    </tr>
    <tr>
        <td>g</td>
        <td>Perform a global match (find all matches rather than stopping after the first match)</td>
    </tr>
    <tr>
        <td>m</td>
        <td>Perform multiline matching</td>
    </tr>
</table>

<br>

### Regular Expression Patterns

**Brackets** are used to find a range of characters:

<table>
	<tr>
		<th>Brackets</th>
		<th>Description</th>
	</tr>
    <tr>
        <td>[abc]</td>
        <td>Find any of the characters between the brackets</td>
    </tr>
    <tr>
        <td>[0-9]</td>
        <td>Find any of the digits between the brackets</td>
    </tr>
    <tr>
        <td>(x|y)</td>
        <td>Find any of the alternatives separated with |
</td>
    </tr>
</table>


<br>

**Metacharacters** are characters with a special meaning:

<table>
	<tr>
		<th>Metacharacters</th>
		<th>Description</th>
	</tr>
    <tr>
        <td>\d</td>
        <td>Find a digit</td>
    </tr>
    <tr>
        <td>\s</td>
        <td>Find a whitespace character</td>
    </tr>
    <tr>
        <td>\b</td>
        <td>Find a match at the beginning or at the end of a word</td>
    </tr>
    <tr>
        <td>\uxxxx</td>
        <td>Find the Unicode character specified by the hexadecimal number xxxx</td>
    </tr>
</table>

<br>

**Quantifiers** define quantities:

<table>
	<tr>
		<th>Quantifiers</th>
		<th>Description</th>
	</tr>
    <tr>
        <td>n+</td>
        <td>Matches any string that contains at least one <em>n</em></td>
    </tr>
    <tr>
        <td>n*</td>
        <td>Matches any string that contains zero or more occurrences of <em>n</em></td>
    </tr>
    <tr>
        <td>n?</td>
        <td>Matches any string that contains zero or one occurrences of <em>n</em></td>
    </tr>
</table>

<br>


