FROM intersystemsdc/irishealth-community:latest

USER root

# Crear el directorio si no existe y dar permisos totales para el Codespace
WORKDIR /home/vscode/workspace
RUN chown -R ${ISC_PACKAGE_MGRUSER}:${ISC_PACKAGE_IRISGROUP} /home/vscode/workspace && \
    chmod -R 777 /home/vscode/workspace

# Volvemos al usuario de IRIS para que el motor arranque correctamente
USER ${ISC_PACKAGE_MGRUSER}
