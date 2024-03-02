# Nike Shoe Dashboard

### Dashboard Link : https://www.novypro.com/project/nike-shoe-dashboard

## Problem Statement
Nike, founded in 1964, is a global leader in athletic footwear. Known for innovation, its shoes cater to various sports with technologies like Air cushioning and Flyknit. Iconic models like Air Max and Jordan transcend sports, becoming fashion symbols. Nike combines performance, style, and sustainability, making its shoes a choice for athletes and fashion enthusiasts worldwide.


This dashboard helps the Nike understand their customers better. It helps the Nike know if their customers are satisfied with their services. Through different ratings, they get to know their improvement area, & thus they can improve their services by identifying these area.



### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that "Images" columns values double quotes (") were replaced with empty values in a column.
- Step 5 : For calculating average #Rating, Here I used the DAX formula "TOPN(100, 'nike_2020_04_13')"
- Step 6 : Since the data contains various images, a new Slicers & New Cards visual were added in the visualizations pane in report view. 
- Step 7 : Visual filters (New Slicers & New Cards) were added for fields named "Product Name", "Images.1", "Images.2", "Images.3", "Images.4" & "Images.5".          
           
           Although, by default, while calculating average, blank values are ignored.
- Step 8 : I've crafted an impressive background page and highlight the visual appeal or aesthetics of the background using Figma tool.        
- Step 9 : New measure was created to find total Sale Price.

Following DAX expression was written for the same,
        
     Total sale price = SUM(nike_2020_04_13[Sale Price])
        
A card visual was used to represent Revenue.

![revenue](https://github.com/santoshsw/Nike-Shoe-Dashboard/assets/107128468/f660a7d7-2d59-44ea-8cb7-3ab8cdecd1f6)

        
 - Step 10 : New measure was created to find  Discount.
 
 Following DAX expression was written to find Discount,
 
         Discount = [Total list price] - [Total sale price]
 
 A card visual was used to represent this Discount.
 
 ![discount](https://github.com/santoshsw/Nike-Shoe-Dashboard/assets/107128468/a2cc58bc-d525-4237-ae63-8306a629cfb3)

 
 - Step 11 : New measure was created to calculate Rating.
 
 Following DAX expression was written to find Rating,
 
         Rating = AVG(nike_2020_04_13[Rating])
    
 A card visual was used to represent this Rating.
 
 
 ![rating](https://github.com/santoshsw/Nike-Shoe-Dashboard/assets/107128468/a7cb0282-ba31-48f6-8e7d-0231ec5f998d)

 - Step 12 : New measure was created to calculate Reviews.

 Following DAX expression was written to find Reviews,

        Review = AVG(nike_2020_04_13[Review])

A card visual was used to represent this Review

 ![review](https://github.com/santoshsw/Nike-Shoe-Dashboard/assets/107128468/76b4b5be-2d97-4364-9636-b307976192c7)
 
 - Step 13 : The report was then published to Power BI Service.
 
 
![publish](https://github.com/santoshsw/Nike-Shoe-Dashboard/assets/107128468/ae2b3775-cf58-40cd-b93e-dc849d85c3b3)

 # Report Snapshot (Power BI DESKTOP)

 
![desktop1](https://github.com/santoshsw/Nike-Shoe-Dashboard/assets/107128468/5e14aa94-5fc7-4d11-a5f3-ec7f4ef0387b)

# 

![desktop2](https://github.com/santoshsw/Nike-Shoe-Dashboard/assets/107128468/8505f142-ebc2-4f5a-90b6-fabc5ffc5a23)

# Snapshot of Dashboard (Power BI Service)

![service](https://github.com/santoshsw/Nike-Shoe-Dashboard/assets/107128468/ba2aa45b-3caa-49b2-a699-aa4cb2eec856)

#

 I took on the challenge of turning a Nike dataset into a Power BI report that's not just informative but visually stunning – almost like browsing a website! 🌐💻 
It's been a blast diving into the world of Nike products and creating a dynamic product viewer for their sneakers. 👟 
I've crafted an impressive background page and highlight the visual appeal or aesthetics of the background using Figma tool.

Now, I want to hear from you! What's your go-to brand, and can you challenge me with your favorite products? 

Let me know in the comments, and give me some inspiration for my next report. ☺️
