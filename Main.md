```local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/ScriptGetter/Main/main/FrenzyUI"))()```

```local Window = Library:CreateWindow("Test Window")```

```local Tab1 = Window:CreateTab("Main")```
```Tab1:CreateButton("Click Me", function()
    print("Button clicked!")
end)```

```Tab1:CreateToggle("God Mode", false, function(state)
    print("God Mode:", state)
end)```

```Tab1:CreateSlider("WalkSpeed", 16, 100, 50, function(value)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = value
end)```

```Tab1:CreateDropdown("Select Gun", {"Pistol", "Shotgun", "Sniper"}, function(choice)
    print("Chosen:", choice)
end)```
