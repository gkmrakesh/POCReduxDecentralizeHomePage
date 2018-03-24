platform :ios, '9.0'
use_frameworks!

def common_pods
    pod 'SwiftLint', '0.24.0'
end

def dependent_pods
    # example - pod 'podname', :git => 'path', :branch => 'development'
end

def example_project
    pod 'HomePage', :path => './'
end

workspace 'HomePage'
target 'HomePage' do
    project 'HomePage.xcodeproj'
    common_pods
    dependent_pods
    example_project
    target 'HomePageTests' do
        inherit! :search_paths
    end
end

target 'HomePageExample' do
    project 'Example/HomePageExample.xcodeproj'
    common_pods
    dependent_pods
    example_project
end
