# Data Considerations

With a system in place, there are additional scope and data-related
variables to consider:

  - **The type and quantity of data –** Are there clustered or pooled
    tables in scope for extraction?  If so, the options available for
    extraction are limited. Consider the number of records and the width
    of tables. For example, with S/4 HANA, SAP has been able to remove
    several tables. However, in some cases, existing tables have become
    wider (300+ columns). 
  - **Frequency of change –** Is the data relatively static (e.g., a
    system configuration table) or changing rapidly (e.g., open items)?
  - **Rate of refresh –** How close to real-time does the data need to
    be to achieve the project’s goals?  For example, are there
    meaningful benefits to the business if data is refreshed every 8
    hours as opposed to every 12 hours?  Data refresh should be
    scheduled for times when the system is not being heavily used.
  - **Security permissions and available connection types –**
    Permissions must be granted to connect to and extract data from
    other systems. The level of access that can be granted to these
    systems affects the design of a solution and the methods for data
    extraction.
