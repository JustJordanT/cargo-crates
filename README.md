# porter-crates
🚢 🏗 a repo for housing crates for porter

![image](https://user-images.githubusercontent.com/38886930/229208345-8452f001-18ba-4246-b080-8bfe9ad2d306.png)

# Crates
a crate is essentially a standardized way of packaging an application or service. It is a Git repository that contains a set of YAML configuration files that define how to install, configure, and run the application. These configuration files include information such as dependencies, environment variables, and executable commands.

When a user wants to use a particular application with Porter, they can simply add the corresponding crate to their configuration by providing the Git repository URL for the crate. Porter will then use the configuration files in the crate to automatically handle the installation and configuration of the application, taking care of any necessary dependencies and settings.

By using crates, Porter provides a modular and extensible approach to managing applications and services. Developers can create and share crates for their own applications, and users can easily add them to their own configurations. This makes it easier to manage complex systems with multiple applications and dependencies, and also allows for greater flexibility and customization in configuring and deploying applications.

An example crate: 

```yaml
name: my_package
version: 1.0.0
download_urls:
  - os: linux
    url: https://example.com/my_package-1.0.0-linux.tar.gz
    sha: abcdef1234567890
  - os: macos
    url: https://example.com/my_package-1.0.0-macos.tar.gz
    sha: abcdef1234567890
  - os: windows
    url: https://example.com/my_package-1.0.0-windows.zip
    sha: abcdef1234567890
```
