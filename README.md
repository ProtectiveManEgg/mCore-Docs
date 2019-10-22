# mCore-Docs

return {
	group = {					-- Group information
		adminHRs = true, 		-- High ranks will be considered admins
		id = 0,					-- Your group ID
		rank = 0,				-- Minimum rank in group to be considered a high rank
		uniform = {
			top = 0,
			bottom = 0,
	},
	admins = {
								-- [name] = id; you don't have to add both
		["ApocalypseManEgg"] = 72915450
	},
	terminal = {
		domination = true,		-- One terminal with both teams able to capture points
		captureTime = 400,		-- How many points, or how much time (minutes) required to win
		totalTime = 1,			-- How long (hours) the server will stay valid for
		defenderMultiplier = 2,	-- How much faster the defenders will rollback the terminal (not for domination-mode)
		required = {			-- How many players required on each team to validate the server
			defenders = 5,
			attackers = 4,
		},
		imgs = {				-- Custom images for under each team's bar in domination-mode
			defenders = 0,
			attackers = 0
		}
	},
	slowmode = {				-- Spam filter for if you're using the custom chat
		enabled = true,
		rate = 2,
	},
	crosshair = nil,			-- Custom image for a crosshair if using the guns
	teams = {					-- Allies team is not required. Set these accordingly
		attackers = "Hostiles",
		defenders = "Defenders",
		allies = "Allies"
	},
	webhook = {					-- Discord webhook to send raid alerts
		channel = "",
		key = ""
	},
	banstore = "",				-- Name of datastore for if you're using the anti-exploit (I recommend you randomize this)
	
	modules = { -- if these are set to false, it should disable the module
		chat = false, 			-- custom chat 
		health = false, 		-- custom health bar
		leaderboard = false,	-- custom player list
		backpack = false,		-- custom backpack/inventory (5 slot hotbar)
		nametag = false,		-- custom overhead nameplates
		loader = false, 		-- load-in gui; class selection, base tour, etc
		terminal = true,
		guns = false,
		admin = false,			-- custom bare-bones admin commands
		animate = false,		-- custom animations
		regions = false, 		-- spawn regions; if a player from the wrong team goes into one, they get respawned
		config = false,			-- the game modifies assets for you; making group updates (like logos) easier
		swords = false,
		turrets = false,
		tanks = false,
		btns = false, 			-- side panel guis
		anti = false, 			-- anti-exploit
	}
}
