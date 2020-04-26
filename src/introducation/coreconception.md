# 一些核心概念

在这一小节中，我会讲几个不难理解但是非常重要的概念。

## 注册

如果你想往Minecraft里添加一些内容，那么你必须做的一件事就是注册。注册是一种机制，告诉游戏本身，有哪东西可以使用。你注册时需要的东西基本上可以分成两个部分：一个注册名和一个实例。

## ResourceLocation

你可以把ResourceLocation想成一种特殊格式的字符串，它大概长成这样:`minecraft:textures/block/stone.png`，一个ResouceLocation指定了资源包下的一个特定的文件。举例来说，前面这个这个ResourceLocation代表了原版资源包下的石头的材质图片。ResouceLocation分成两部分，冒号前面的叫做「域（domain）」，在原版中只有一个域即`minecraft`域，但是如果你开始开发mod，那么每个mod都会有一个或者多个域。冒号的后半部分是和`asserts`文件夹内的目录结构一一对应的。从某种程度上来说，ResourceLocation就是一个特殊的URL。

## 模型和材质

在游戏中3d的对象都是基本上都有它的模型，模型和材质组合在一起规定了一个对象具体的样子。模型相当于是骨头，材质相当于是皮肤。在大部分时候，你的材质都是png图片，请注意保证你的材质背景是透明的，其次不要在材质中使用半透明像素，会有不可预知的问题。