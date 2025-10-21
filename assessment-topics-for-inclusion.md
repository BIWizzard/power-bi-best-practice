Hi Ken,  In the work with Thomas at AbsoluteCare did you guys discuss any priorities for report optimization?
 
Hey Ross,
 
The primary optimization recommendation was switching all reports to Import - which they implemented across all reports.
 
As far as roadmap priorities we have discussed:
Normalizing data model/moving away from 1 big table

- identifying foundational dimensions - Members, locations, payers, etc...

   - I suggested, if allowable, to create a schema in existing source SQL DB, and take their best shot at building out some key dimensions as views, and use those to build data models/star schema as opposed to the "One Big Table" views and native queries they are using.  These assets can be helpful in future scoping and architecture planning and will improve their semantic model now.

- Identifying Source of Truth for each i.e. if I need a list of all active members, where do I get it?

- Creating a standard date table/dimension used across all reports to support Time Intelligence functions.  I suggested this was one of items they could do "now", in Power BI layer,  in parallel to any broader architecture planning.  What they create now could end up being long term solution, a template for date dimension in EDW, or a scoping conversation started.

- Measure rigor:  

   -Use measure tables and dynamic folders to organize measures 

   -Stop using implicit measures

   -Use variables

   -Use measure chaining - build modular, repeatable stuff

- Field Parameters and Bookmarks - How to and Use Cases

- UI/UX stuff:

   - Use empty space - let stuff breathe

   - Color Psychology - colors have meaning - limit if not using as indicators

   - Navigation - intuitive, familiar, web app feel

Outside of that - have just reinforced creating reusable components, style guide, templates to remove cognitive load, decisions when building new reports - same look an feel across all reports and apps.  Have discussed they are kind of "tip of the spear" and their voices will be very important and their architecture in re-engineered.  The know the data, what the data consumers are asking for, what they measure regularly.  They can really help process by documenting their existing systems and processes and being ready to discuss needs and designing new objects and defining future semantic model...

Thats probably more than you were asking for...Hope it helps.  Let me know if you want to talk through any of it in more detail...

 
 