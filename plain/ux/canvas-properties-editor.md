#Canvas Properties
--------------------

- __Canvas Info__
	- Name
	- Description
- __Image__
	- Image Size
		- Width / Height
		- XRes / Y Res
		- Physical Width / Physical Height
		- Image Span
	- Image Area
		- Top Left X / Y
		- Bottom X / Y 
- __Time__
	- Frames per second
	- Start time
	- End time
	- Duration	
- __Other__
	- Locks and Links
		- Image Width / Height / Aspect / Span
		- Pixel Width / Height / Aspect
	- Focus Point
		- Focus Point X / Y
	
	
#Canvas Options
-----------------

- __Grid__
	- Grid size X / Y
	- Show grid
	- Snap to grid
- __Time__
	- Snap to frame
- __Units__
	- Not yet implemented
	
	

#Questions
----------
- What is physical width/height?  

- What is image span?  

- What is image area?  
it seems like origin point of coordinate of canvas
- What is Locks and Links?  

- What is Focus Points?  

- Canvas Options is not yet ready for final users, shall we remove them till they are implemented completely and properly?  
When saying completely and properly, I mean we need to design (UI and UX) and then code them down, test, publish to end users.

#Canvas Properties Editor Proposal
------------------------
- __Canvas Info__
	- Name
	- Description  
	should be in multi-line instead of single line.  
	And for a long term, XMP intigration is welcome very much!
- __Canvas Size__
	- `Width / Height`  
	there is a preset avaible
	- `Resoultions X / Y`  
	X and Y are linked by default
	- `Origin Point`  
	positon of the canvas point to (0,0), provide 9 buttons for quick setup:  
		
		| 1 | 4 | 7 |
		|---|---|---|
		| 2 | 5 | 8 |
		| 3 | 6 | 9 |
		
		- Button 1 (Left, Top)
		- Button 2 (Left, Middle)
		- Button 3 (Left, Bottom)
		- Button 4 (Middle, Top)
		- Button 5 (Middle, Middle)
		- Button 6 (Middle, Bottom)
		- Button 7 (Right, Top)
		- Button 8 (Right, Middle)
		- Button 9 (Right, Bottom)
	- `Time`
		- FPS, Start and End time, Duration 
- __Advanced Settings__
	- `Locks and Links`
	- `Focus Point X/Y`
	- And `other things` in most cases user don’t want to change from time to time.  
	_I am not sure if metadata is recorded in sif document, if yes, we can attach those parameters in here too, so that we migrate Canvas Options to `Canvas Properties Editor`._