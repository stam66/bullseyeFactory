# bullseyeGenerator
LiveCode IDE plugin  to create a bullseye for left ventricular assessment for cardiology projects

Generate Bullseye displays of any size for LV assessment in cardiology. 
To install as plugin, drop in your plugins folder and restart LiveCode. To use, choos a diameter/width for the bullseye display and click "create" - this copies the new bullseye into the clipoard to past in the mainstack.

<img width="755" alt="Screenshot 2022-12-06 at 02 41 11" src="https://user-images.githubusercontent.com/5677273/205797579-83fe3157-f6ae-474e-b4ca-71ae8c351211.png">

The model is a 16/17 segment model in accordance with [AHA/EACVI guidlines](https://asecho.org/wp-content/uploads/2015/01/ChamberQuantification2015.pdf).
Click any segment to score each segment in as per the guideline above.
Calculates WMSI and LVEF based on wall motion scores based on 2 separate published algorithms (references included in the code). Values are stored as custom properties of the grup as uWMSI, uLVEF1, uLVEF2. All segmental scores are stored as an ordered comma-seperated list of scores (corresponding to each segment), stored internally as the uScores of group.

To retrieve the scores: get the uScores of group "bullseye"; setting the uScores (or any indvidual score) updates the custom property, color display and  
Buttons on the left score all segments as either normal, hypokinetic, akinetic, dyskinetic/aneurysmal or uninterpretable and changes can be made on top of this, or reset all to unread.

The Cog wheel icon shows/hides additional setting such as displaing calculations, show/hide wall names and choosing 16 or 17 segment model.

MIT licence - the copyright notice must follow all distribution/derivative works.
