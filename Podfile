platform :ios, '13.0'

target 'food-market-ios' do
  use_frameworks!

  pod 'DropDown', '2.3.13'

  # Force all pod targets to use iOS 13
  post_install do |installer|
    installer.pods_project.targets.each do |target|
      target.build_configurations.each do |config|
        config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '13.0'
      end
    end
  end
end
