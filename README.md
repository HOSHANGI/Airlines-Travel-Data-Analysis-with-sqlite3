# Airlines-Travel-Data-Analysis-with-sqlite3

https://acrobat.adobe.com/link/review?uri=urn:aaid:scds:US:14e66ac0-33b1-4a49-9d3f-f60e6b769342

tickets = pd.read_sql_query("""select * from tickets inner join bookings on tickets.book_ref = bookings.book_ref""", connection) tickets['book_date'] = pd.to_datetime(tickets['book_date']) tickets['date'] = tickets['book_date'].dt.date x = tickets.groupby('date')[['date']].count()  plt.figure(figsize = (18,6)) plt.plot(x.index, x['date'],marker = '^') plt.xlabel('Date', fontsize = 20) plt.ylabel('Number of Tickets', fontsize = 20) plt.grid('b') plt.show() 

To summarize, analyzing revenue data such as total revenue per year,
average revenue per ticket, and average occupancy per aircraft is critical
for airlines seeking to maximize profitability. Airlines can find areas for
improvement and modify their pricing and route plans as a result of
assessing these indicators. A greater occupancy rate is one important
feature that can enhance profitability since it allows airlines to maximize
revenue while minimizing costs associated with vacant seats. The airline
should revise the price for each aircraft as the lower price and high price is
also the factor that people are not buying tickets from those aircrafts. They
should decide the reasonable price according to the condition and facility of
the aircraft and it should not be very cheap or high.
Furthermore, boosting occupancy rates should not come at the price of
consumer happiness or safety. Airlines must strike a balance between the
necessity for profit and the significance of delivering high-quality service
and upholding safety regulations. Airlines may achieve long-term success
in a highly competitive business by adopting a data-driven strategy to
revenue analysis and optimisation

![download (2)](https://github.com/HOSHANGI/Airlines-Travel-Data-Analysis-with-sqlite3/assets/118753140/8af01cdc-711d-4bfc-9d98-20695461dc38)
![download (1)](https://github.com/HOSHANGI/Airlines-Travel-Data-Analysis-with-sqlite3/assets/118753140/10970f90-71f7-4885-800c-316db9b73931)
![download](https://github.com/HOSHANGI/Airlines-Travel-Data-Analysis-with-sqlite3/assets/118753140/f4fa7e5a-b183-4e0a-9e37-abfe543066fb)
