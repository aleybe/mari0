# STEM Demo

![](https://j.gifs.com/RO17RR.gif)

## Demo Code

```lua
function mario:changeColor(dt)
	
	-- MARIO COLORS --
	------------------
	--1: hat, pants (red)
	--2: shirt, shoes (brown-green)
	--3: skin (yellow-orange)

	timeToChange = 1

	self.currentTimeSince = self.currentTimeSince + dt

	if self.currentTimeSince > timeToChange then

		customColor = {{math.random(0, 255)/255, math.random(0, 255)/255, math.random(0, 255)/255},
					   {math.random(0, 255)/255, math.random(0, 255)/255, math.random(0, 255)/255}, 
					   {math.random(0, 255)/255, math.random(0, 255)/255, math.random(0, 255)/255}}
		
		changingcolors = {customColor[1], customColor[2], customColor[3]}

		self.colors = changingcolors
		self.currentTimeSince = 0
	end

end 
```


# mari0
Runs on LÖVE 11.2

MIT License

Forked from the original repo by Maurice Guégan