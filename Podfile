# Uncomment the next line to define a global platform for your project
platform :ios, '15.0'

target 'MyApp' do
  use_frameworks!

pod 'Appirater'
pod 'SDWebImage'

# Firebase
pod 'Firebase/Core'
pod 'Firebase/Auth'
pod 'Firebase/Database'
pod 'Firebase/Analytics'
pod 'Firebase/Crashlytics'
pod 'Firebase/Storage'
pod 'Firebase/Firestore'
pod 'FirebaseFirestoreSwift'

post_install do |installer|
  installer.pods_project.targets.each do |target|
    
    target.build_configurations.each do |config|
    config.build_settings['EXCLUDED ARCHS[sdk=iphonesimulator*]'] = "i386"
    end
    
    if target.name == 'BoringSSL-GRPC'
      target.source_build_phase.files.each do |file|
        if file.settings && file.settings['COMPILER_FLAGS']
          flags = file.settings['COMPILER_FLAGS'].split
          flags.reject! { |flag| flag == '-GCC_WARN_INHIBIT_ALL_WARNINGS' }
          file.settings['COMPILER_FLAGS'] = flags.join(' ')
        end
      end
    end
  end
end

end

