# Precedence

The simplest optimization that can be made to most pages is control view
record reduction. UCVs and DCVs are usually the biggest offenders of
unnecessarily large record sets.

The majority of the time a DCV is created, it selects the entire record
set and does something like:

<span style="font-family: &#39;Courier New&#39;;">SELECT CASE WHEN
\[Field\] = 1</span>

<span style="font-family: &#39;Courier New&#39;;">THEN 0
--Disabled</span>

<span style="font-family: &#39;Courier New&#39;;">ELSE 1 --
Enabled</span>

<span style="font-family: &#39;Courier New&#39;;">END as
\[Enabled\]</span>

<span style="font-family: &#39;Courier New&#39;;">FROM \[Table\] WHERE
\[Field\]</span>

However, DCV’s do not require every record to be present. If it’s
expected that more than often records will be DISABLED as opposed to
ENABLED the DCV should change to:

<span style="font-family: &#39;Courier New&#39;;">SELECT 1 as
\[Disabled\] FROM \[Table\] WHERE \[Field\] \<\> 1</span>

where the Control Status is set to Enabled by default within the pages
configuration.

This does several things:

  - Reduces the record set site, improving performance

  - Reduces the complexity of the view, improving performance

  - Simplifies the view, making it easier to understand
