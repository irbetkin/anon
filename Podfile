# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'AnonTest' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

  # Pods for AnonTest
#Architecture pods
   pod 'PluggableApplicationDelegate'
   pod 'Swinject'
   pod 'SwinjectStoryboard', "~> 2.2.0"
   pod "PromiseKit", "~> 6.8"


#network
   pod 'Alamofire', '~> 4.7'
   pod 'Alamofire-SwiftyJSON'
   pod 'SDWebImage'
   
  target 'AnonTestTests' do
    inherit! :search_paths
    # Pods for testing
  end

end
post_install do |installer|
	installer.pods_project.targets.each do |target|
		if target.name == 'PluggableApplicationDelegate'
			target.build_configurations.each do |config|
				config.build_settings['SWIFT_VERSION'] = '4.0'
			end
		end
	
	end
end
