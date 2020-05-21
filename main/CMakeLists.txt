# Embed the server root certificate into the final binary
idf_build_get_property(project_dir PROJECT_DIR)
idf_component_register(SRCS "main.c" "MyWiFi.c" "OTAServer.c"
                    INCLUDE_DIRS "."
                    EMBED_TXTFILES ${project_dir}/main/WebsiteFiles/favicon.ico ${project_dir}/main/WebsiteFiles/index.html ${project_dir}/main/WebsiteFiles/jquery-3.3.1.min.js  ${project_dir}/main/WebsiteFiles/jquery-3.4.1.min.js)
