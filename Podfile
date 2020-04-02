# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

is_running_in_renovate = ENV['HOME'] == '/home/ubuntu'
if is_running_in_renovate
  install! 'cocoapods', :integrate_targets => false
else
  install! 'cocoapods'
end

target 'RenovateCocoaPodsSample' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!

  # https://github.com/CocoaPods/CocoaPods/issues/8653#issuecomment-488767262
  current_target_definition.swift_version = '5.0'

  # Pods for RenovateCocoaPodsSample
  pod 'Alamofire', '5.0.0'
  pod 'RxSwift', '~> 5.0.0'
  pod 'KeychainAccess', '~> 4.0'
end
