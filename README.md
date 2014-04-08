SharePoint-Hide-Open-With-Explorer
==================================

SharePoint solution the hide the Open with Explorer option in the Ribbon

# Installation

	Add-SPSolution .\SharePoint-Hide-Open-With-Explorer\HideExplorer\bin\Debug\HideExplorer.wsp
	Install-SPSolution -Identity (Get-SPSolution | Where-Object{$_.Name -like "hideexplorer.wsp"}).SolutionId.Guid -GACDeployment
	
Now you should be able to activate the solution as a site collection feature.