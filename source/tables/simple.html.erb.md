---
title: Simple Tables
status: editors-draft
technologies: HTML5
order: 2
---

A simple table has one header row and/or header column.

Use header cell elements (`<th>`) to markup the header cells so that they are distinguishable from data cells and associated with the correct data cells.
For example, in the second table below "Closed" is meaningless on its own, but makes sense when it is associated
with the time (the row header) and the date (the column header).

Additionally, `<caption>` elements may be used to identify a table in the document which is a way for meeting WCAG 2.0 requirements in [specific situations](caption-summary.html).

## Table with header cells in the top row only
{:.ex}

This table of concert dates only needs the cells in the top row marked up as `<th>` cells. This is partly because it is such a small table and partly because the data itself is distinctly different in each column.

{::nomarkdown}
<%= sample_start %>

<p><strong>Concert dates:</strong></p>
<table>
	<tr>
		<th>Date</th>
		<th>Event</th>
		<th>Venue</th>
	</tr>
	<tr>
		<td>12 Feb</td>
		<td>Waltz with Strauss</td>
		<td>Main Hall</td>
	</tr>
	<tr>
		<td>24 Mar</td>
		<td>The Obelisks</td>
		<td>West Wing</td>
	</tr>
	<tr>
		<td>14 Apr</td>
		<td>The What</td>
		<td>Main Hall</td>
	</tr>
</table>

<%= sample_end %>
{:/nomarkdown}

{::nomarkdown}
<%= code_start %>
{:/nomarkdown}

~~~ html
<table>
	<tr>
		<th>Date</th>
		<th>Event</th>
		<th>Venue</th>
	</tr>
	<tr>
		<td>12 Feb</td>
		<td>Waltz with Strauss</td>
		<td>Main Hall</td>
	</tr>
	[…]
</table>
~~~

{::nomarkdown}
<%= code_end %>
{:/nomarkdown}

[Full code for “Table with header cells in the top row only”](examples/headertoprow.html)

## Table with header cells in the top row and first column
{:.ex}

This table of opening times has header information contained in both the top row and the first column. All header cells are marked up as `<th>` cells.

{::nomarkdown}
<%= sample_start %>

<table>
	<tr>
		<th>Delivery slots</th>
		<th>Monday</th>
		<th>Tuesday</th>
		<th>Wednesday</th>
		<th>Thursday</th>
		<th>Friday</th>
	</tr>
	<tr>
		<th>09:00 - 11:00</th>
		<td>Closed</td>
		<td>Open</td>
		<td>Open</td>
		<td>Closed</td>
		<td>Closed</td>
	</tr>
	<tr>
		<th>11:00 - 13:00</th>
		<td>Open</td>
		<td>Open</td>
		<td>Closed</td>
		<td>Closed</td>
		<td>Closed</td>
	</tr>
	<tr>
		<th>13:00 - 15:00</th>
		<td>Open</td>
		<td>Open</td>
		<td>Open</td>
		<td>Closed</td>
		<td>Closed</td>
	</tr>
	<tr>
		<th>15:00 - 17:00</th>
		<td>Closed</td>
		<td>Closed</td>
		<td>Closed</td>
		<td>Open</td>
		<td>Open</td>
	</tr>
</table>

<%= sample_end %>
{:/nomarkdown}

{::nomarkdown}
<%= code_start %>
{:/nomarkdown}

~~~ html
<table>
	<tr>
		<th>Delivery slots</th>
		<th>Monday</th>
		<th>Tuesday</th>
		<th>Wednesday</th>
		<th>Thursday</th>
		<th>Friday</th>
	</tr>
	<tr>
		<th>09:00 - 11:00</th>
		<td>Closed</td>
		<td>Open</td>
		<td>Open</td>
		<td>Closed</td>
		<td>Closed</td>
	</tr>
	<tr>
		<th>11:00 - 13:00</th>
		<td>Open</td>
		<td>Open</td>
		<td>Closed</td>
		<td>Closed</td>
		<td>Closed</td>
	</tr>
	[…]
</table>
~~~

{::nomarkdown}
<%= code_end %>
{:/nomarkdown}

[Full code for “Table with header cells in the top row and first column”](examples/headertoprowfirstcol.html)

## Related WCAG2.0 Techniques

The following WCAG 2.0 technique was used in the examples above:

-   [H51: Using table markup to present tabular data](http://www.w3.org/TR/WCAG20-TECHS/H51)
