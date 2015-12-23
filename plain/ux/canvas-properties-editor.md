#Canvas Properties

- Canvas Info
	- Name
	- Description
- Image
	- Image Size
		- Width / Height
		- XRes / Y Res
		- Physical Width / Physical Height
		- Image Span
	- Image Area
		- Top Left X / Y
		- Bottom X / Y 
- Time
	- Frames per second
	- Start time
	- End time
	- Duration	
- Other
	- Locks and Links
		- Image Width / Height / Aspect / Span
		- Pixel Width / Height / Aspect
	- Focus Point
		- Focus Point X / Y
	
	
#Canvas Options

- Grid
	- Grid size X / Y
	- Show grid
	- Snap to grid
- Time
	- Snap to frame
- Units
	- Not yet implemented
	
	

#Questions
- What is physical width/height?  

- What is image span?  

- What is image area?  
it seems like origin point of coordinate of canvas
- What is Locks and Links?  

- What is Focus Points?  

- Canvas Options is not yet ready for final users, shall we remove them till they are implemented completely and properly?  
When saying completely and properly, I mean we need to design (UI and UX) and then code them down, test, publish to end users.

#Canvas Properties Editor Proposal
- Canvas Info
	- Name
	- Description  
	should be in multi-line instead of single line.  
	And for a long term, XMP intigration is welcome very much!
- Canvas Size 
	- Width / Height  
	there is a preset avaible
	- Resoultions X / Y  
	X and Y are linked by default
	- Origin Point  
	positon of the canvas point to (0,0)  
	provide 9 buttons for quick setup:  
		
		| 1 | 4 | 7 |
		|---|---|---|
		| 2 | 5 | 8 |
		| 3 | 6 | 9 |
		
		- 1 (Left, Top)
		- 2 (Left, Middle)
		- 3 (Left, Bottom)
		- 4 (Middle, Top)
		- 5 (Middle, Middle)
		- 6 (Middle, Bottom)
		- 7 (Right, Top)
		- 8 (Right, Middle)
		- 9 (Right, Bottom)
	- Time
		- FPS, Start and End time, Duration 
- Advanced Settings ()
	- Locks and Links
	- Focus Point X/Y
	- And other things in most cases user don’t want to change from time to time.  
	I am not sure if metadata is recorded in sif document, if yes, we can attach those parameters in here too, so that we migrate Canvas Options to Canvas Properties Editor.