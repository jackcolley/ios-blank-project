# Uncomment the next line to define a global platform for your project
platform :ios, '9.0'

def common_pods
    pod 'Alamofire', '~> 4.0'
    pod 'JSONJoy-Swift', '~> 2.1.0'
    pod 'Heimdallr', :git => 'https://github.com/marcelofabri/Heimdallr.swift.git', :branch => 'swift-3.0'
    pod 'AlamofireNetworkActivityIndicator', '~> 2.0'
    pod 'IQKeyboardManagerSwift'
    pod 'FontAwesome.swift', :git => 'https://github.com/thii/FontAwesome.swift.git', :branch => 'master'
    pod 'SVProgressHUD'
    pod 'SwiftyAttributes'
    pod 'Pluralize.swift', :git => 'https://github.com/joshualat/Pluralize.swift.git', :branch => 'master'
end
target 'blank-project' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

  # Pods for blank-project
    common_pods

  target 'blank-projectTests' do
    inherit! :search_paths
    # Pods for testing
    common_pods
  end

end
