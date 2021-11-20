idf_component_register(SRCS "proj4.c"
                    INCLUDE_DIRS "."
                    EMBED_TXTFILES  "certs/ClientCert.pem"
                                    "certs/ServerCert.pem"
                                    "certs/ServerKey.pem")
