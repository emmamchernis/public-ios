source 'https://github.com/CocoaPods/Specs.git'

# Uncomment this line to define a global platform for your project
platform :ios, '8.0'
# Uncomment this line if you're using Swift
use_frameworks!

target 'iOSMinimalCocoaPodsSample' do
  pod 'AFNetworking', '~> 3.0'
  pod 'ORStackView', '~> 3.0'
  pod 'SwiftyJSON', '~> 4.0'
  pod 'Parse', :git => 'https://github.com/ParsePlatform/Parse-SDK-iOS-OSX.git', :commit => '931684b3dce25ec447d3df38b02e988970663c24'
end

target 'iOSMinimalCocoaPodsSampleTests' do

end

target 'iOSMinimalCocoaPodsSampleUITests' do

end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['SWIFT_VERSION'] = '4.0'
      config.build_settings['MACOSX_DEPLOYMENT_TARGET'] = '10.10'
    end
  end
end
