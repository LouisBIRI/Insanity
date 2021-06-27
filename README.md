<Settings>
	<!-- 
	Awake Type Explanation:
	name -> The name to display inside of the bot when choosing the awake (Example: ADOCH)
	gametext -> Case-sensitive awake line text inside of the game (Example: Additional Damage of Critical Hits) 
	comparisonmethod -> An additional attribute to modify which method an awake is compared with. Options are Exact and Contains. Exact is default.
						Example <Type name="INT" gametext="INT" comparisonmethod="Contains" text_to_find="NT"></Type>
						
						"Contains" compares by checking if the read awake contains the value in text_to_find
						"Exact" does an exact case insensitive comparison (this is the default and preferred)
					
	text_to_find -> If using comparison method Contains, then text_to_find is the value to find within the awake text.
	-->
	<AwakeTypes>  
		<Type name="INT" gametext="INT"></Type>
		<Type name="DEX" gametext="DEX"></Type>
		<Type name="STR" gametext="STR"></Type>
		<Type name="STA" gametext="STA"></Type>
		<Type name="ADOCH" gametext="ADOCH"></Type>
		<Type name="Increased Attack" gametext="Increased Attack"></Type>
		<Type name="Increased HP" gametext="Increased HP"></Type>
		<Type name="Increased MP" gametext="Increased MP"></Type>
		<Type name="Attack" gametext="Attack"></Type>
		<Type name="PvE Damage" gametext="PvE Damage Increase"></Type>
		<Type name="Increased DEF" gametext="Increased DEF"></Type>
		<Type name="DEF" gametext="DEF"></Type>
		<Type name="Critical Chance" gametext="Critical Chance"></Type>
		<Type name="Attack Speed" gametext="Attack Speed"></Type>
		<Type name="DCT" gametext="Decreased Casting Time"></Type>
		<Type name="EXP" gametext="EXP"></Type>
		<Type name="Speed" gametext="Speed"></Type>
		<Type name="Max HP" gametext="Max. HP"></Type>
		<Type name="Max MP" gametext="Max. MP"></Type>
		<Type name="Max FP" gametext="Max. FP"></Type>
	</AwakeTypes>

	<!-- 
	The color of a pixel in the in-game awake line text. 
	Format: RGB (R, G, B) 
	
	Adding multiple awake colors example:
	<Setting name="AwakeTextPixelColorRgb">0, 255, 0</Setting>
	<Setting name="AwakeTextPixelColorRgb1">0, 0, 255</Setting>
	<Setting name="AwakeTextPixelColorRgb2">245, 0, 0</Setting>
	<Setting name="AwakeTextPixelColorRgb3">0, 0, 185</Setting>
	
	The above example of multiple awake colors will find awakes with all of those pixel colors
	You can add as many as you want. 
	It requires the format as above: AwakeTextPixelColorRgb, AwakeTextPixelColorRgb1, AwakeTextPixelColorRgb2... and so on.
	
	Adding a range of pixel colors:
	<Setting name="AwakeTextPixelColorRgb">0, 245-255, 0</Setting>
	
	The above example will stop when the pixel color is between 0, 245, 0 and 0, 255, 0
	It will stop at 0, 251, 0 as an example.
	-->
	<Setting name="AwakeTextPixelColorRgb">0, 255, 0</Setting>
  
	<!-- 
	The amount of time in milliseconds it takes before an awake scroll is done
	showing that "Watering Effect" on the item before awakening it 
	-->
	<Setting name="ScrollDelayMs">200</Setting>
  
	<!-- 
	The value for Language is the name of the .traineddata file.
	Example eng.traineddata, then the value is eng
			por.traineddata, then the value is por
	-->
	<Setting name="Language">eng</Setting>
  
	<!-- 
	Words that are ignored when the OCR engine reads the awake
	NOTE: Do not add a space after comma, the space counts as part of the word 
	Format: Word1,Word2,Word3
	-->
	<Setting name="OcrIgnoreWords">Blessing Options</Setting>
</Settings>

