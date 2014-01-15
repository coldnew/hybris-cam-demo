cmake_minimum_required (VERSION 2.8) 
project(hybris-cam-demo) 


include_directories(${CMAKE_CURRENT_SOURCE_DIR})

add_executable (hybris-cam-demo-gui direct_camera_test_gui.cpp)
target_link_libraries ( hybris-cam-demo-gui  
                       	/usr/lib/arm-linux-gnueabihf/libcamera.so
        		/usr/lib/arm-linux-gnueabihf/libis.so
		        #/usr/lib/arm-linux-gnueabihf/libhybris-common.so

                        #/usr/lib/arm-linux-gnueabihf/libGLESv2.so
			/usr/lib/arm-linux-gnueabihf/libhybris-egl/libGLESv2.so.2                        

			#/usr/lib/arm-linux-gnueabihf/libEGL.so
			/usr/lib/arm-linux-gnueabihf/libhybris-egl/libEGL.so.1
			
			/usr/lib/arm-linux-gnueabihf/libui.so
			/usr/lib/arm-linux-gnueabihf/libhardware.so
			
			/usr/lib/arm-linux-gnueabihf/libsf.so
)

