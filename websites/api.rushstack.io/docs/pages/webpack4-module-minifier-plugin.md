---
hide_title: true
custom_edit_url: null
pagination_prev: null
pagination_next: null
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@rushstack/webpack4-module-minifier-plugin](./webpack4-module-minifier-plugin.md)

## webpack4-module-minifier-plugin package

## Classes

| Class                                                                                                   | Description                                                                                                                                                                                                                                                                                                 |
| ------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [ModuleMinifierPlugin](./webpack4-module-minifier-plugin.moduleminifierplugin.md)                       | Webpack plugin that minifies code on a per-module basis rather than per-asset. The actual minification is handled by the input <code>minifier</code> object.                                                                                                                                                |
| [PortableMinifierModuleIdsPlugin](./webpack4-module-minifier-plugin.portableminifiermoduleidsplugin.md) | Plugin responsible for converting the Webpack module ids (of whatever variety) to stable ids before code is handed to the minifier, then back again. Uses the node module identity of the target module. Will emit an error if it encounters multiple versions of the same package in the same compilation. |

## Functions

| Function                                                                                                                             | Description                                                                                                                                          |
| ------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| [generateLicenseFileForAsset(compilation, asset, minifiedModules)](./webpack4-module-minifier-plugin.generatelicensefileforasset.md) | Generates a companion asset containing all extracted comments. If it is non-empty, returns a banner comment directing users to said companion asset. |
| [rehydrateAsset(asset, moduleMap, banner)](./webpack4-module-minifier-plugin.rehydrateasset.md)                                      | Rehydrates an asset with minified modules.                                                                                                           |

## Interfaces

| Interface                                                                                         | Description                                                                       |
| ------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| [IAssetInfo](./webpack4-module-minifier-plugin.iassetinfo.md)                                     | Information about a dehydrated webpack ECMAScript asset                           |
| [IDehydratedAssets](./webpack4-module-minifier-plugin.idehydratedassets.md)                       | The set of data remaining to rehydrate in the current compilation                 |
| [IExtendedModule](./webpack4-module-minifier-plugin.iextendedmodule.md)                           | Extension of the webpack Module typings with members that are used by this Plugin |
| [IModuleInfo](./webpack4-module-minifier-plugin.imoduleinfo.md)                                   | Information about a minified module                                               |
| [IModuleMinifierPluginHooks](./webpack4-module-minifier-plugin.imoduleminifierpluginhooks.md)     | Hooks provided by the ModuleMinifierPlugin                                        |
| [IModuleMinifierPluginOptions](./webpack4-module-minifier-plugin.imoduleminifierpluginoptions.md) | Options to the ModuleMinifierPlugin constructor                                   |
| [IPostProcessFragmentContext](./webpack4-module-minifier-plugin.ipostprocessfragmentcontext.md)   | Argument to the postProcessCodeFragment hook for the current execution context    |

## Variables

| Variable                                                                            | Description                                                                                                                                                                                                          |
| ----------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [CHUNK_MODULES_TOKEN](./webpack4-module-minifier-plugin.chunk_modules_token.md)     | Token to replace the object or array of module definitions so that the minifier can operate on the Webpack runtime or chunk boilerplate in isolation                                                                 |
| [MODULE_WRAPPER_PREFIX](./webpack4-module-minifier-plugin.module_wrapper_prefix.md) | Prefix to wrap <code>function (module, **webpack_exports**, **webpack_require**) { ... }</code> so that the minifier doesn't delete it. Public because alternate Minifier implementations may wish to know about it. |
| [MODULE_WRAPPER_SUFFIX](./webpack4-module-minifier-plugin.module_wrapper_suffix.md) | Suffix to wrap <code>function (module, **webpack_exports**, **webpack_require**) { ... }</code> so that the minifier doesn't delete it. Public because alternate Minifier implementations may wish to know about it. |
| [STAGE_AFTER](./webpack4-module-minifier-plugin.stage_after.md)                     | Stage \# to use when this should be the last tap in the hook                                                                                                                                                         |
| [STAGE_BEFORE](./webpack4-module-minifier-plugin.stage_before.md)                   | Stage \# to use when this should be the first tap in the hook                                                                                                                                                        |

## Type Aliases

| Type Alias                                                    | Description                                |
| ------------------------------------------------------------- | ------------------------------------------ |
| [IAssetMap](./webpack4-module-minifier-plugin.iassetmap.md)   | A map from file names to dehydrated assets |
| [IModuleMap](./webpack4-module-minifier-plugin.imodulemap.md) | A map from module ids to minified modules  |