local directions = {"Forward", "Left", "Right"}

while true do
  
    for _, direction in pairs(directions) do
      
        local args = {
            [1] = direction
        }
        
      
        game:GetService("ReplicatedStorage").Rounds.Core.Default.Remotes.Pass:InvokeServer(unpack(args))
    end
end
