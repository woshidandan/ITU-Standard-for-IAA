# ITU-Standard-for-IAA
After three years of discussion and revision, the first international standard on image aesthetics assessment metadata, which I spearheaded, has been published. 经过三年的讨论和修改，由我主持的首个关于图像美学评估元数据的国际标准发布.

# Summary
Sometimes, you may want to take a nice photo, but before that, we need to know what is the key to the beauty of the image. In fact, with the development of the market economy, and the improvement of people's spiritual and cultural needs, our mobile terminal manufacturers not only need to provide better device to take photos, but also need to know whether the image cat to most users' preference. There are already many objective evaluation standards to help us select an excellent mobile terminal device, but an excellent device may not be able to take beautiful photos. For applications in which images are ultimately to be viewed by human beings, the only “correct” method of quantifying visual image aesthetics, is through subjective evaluation. However, the relevant standards on subjective evaluation of images in mobile terminal are still blank.

Subjective evaluation aims to evaluate whether the image conforms to the possible audience's aesthetics, which belongs to the scope of image aesthetics assessment (hereinafter called IAA). On the one hand, the aesthetic attributes and the processes that affect the final image aesthetics are complex, so the industry lacks a unified definition for it; on the other hand, due to the spiritual and cultural differences among users, even for the same image, there are a thousand Hamlets in a thousand people's eyes. Therefore, we are not yet able to make a fast and effective subjective evaluation.

Maybe, we can seek help from artificial intelligence algorithms. The essence of IAA is to quantify aesthetics, when we use AI algorithms, it mainly includes two methods: one is to evaluate the overall aesthetics of the image, and the other is to evaluate aesthetics based on multiple aesthetic attributes. We prefer to use multiple aesthetic attributes to evaluate images, which are more comprehensive, but we found that current datasets are far from meeting the requirements of AI algorithms, due to various problems. As everyone knows, AI is driven by data, but we have no high-quality data. The main reason is that the existing standards cannot regulate the content of IAA and guide the establishment of IAA metadata. 

![image](https://github.com/woshidandan/ITU-Standard-for-IAA/assets/15050507/23ab78f7-2a24-4e2e-a470-94d0cb7c9df4)

In order to solve the above problems, this standard proposes a method for constructing IAA metadata, it divides the dimensions involved in IAA from the perspective of the role (photographer, camera, viewer), while also providing the aesthetic attributes of each dimension.

Beauty comes from life, our standard comes from the process of image generation to the final aesthetic evaluation. Let's take a look at Figure 1, please imagine, you want to use the camera to record something beautiful, the first step, even as a non-professional photographer, you may want to adjust the angle of the shot, select a good composition, then, the second step, you adjust the camera exposure and press the shutter button, your camera gives you an image. Maybe you are not sure how this image looks like, you post it to your Instagram and invite your friends to comment on it. This process involves three key roles, you are the Photographer, you may use some photography techniques to select a good composition, your Camera, the camera may give a good exposure degree, and your friends are the Viewer, they will evaluate this image based on their preferences. These roles and attributes work together to affect the image aesthetics you get.

The role-based metadata defined in this standard, will provide support for the following aspects:
1)	First, it can effectively guide the construction of IAA datasets, these datasets can be used to drive aesthetic algorithms.
2)	Second, it can promote IAA to be used in more practical products, and improve the cultural orientation and additional value of the product.
3)	Third, it can fill the gap of standards in the direction of subjective image evaluation,  standardize industry IAA tasks, and improve the mobile terminal computational photography system series standards.

# 简介
随着用户日益增长的精神文化需求，目前的移动终端计算摄影系统，不仅要求设备在拍照时采集到高质量的影像，还需要解决如何将被摄对象表现得更美的问题，前者可通过图像客观评测来检测质量，后者可利用图像主观评测来评估美感。在图像的客观评测方面，一些较为著名行业标准或系统，如CPIQ IEEE P1858，DxOmark，VCX等，和一些用于单因素的评测标准，如Exposure (ISO 12232)，Dynamic range and noise (ISO 15739)，Color shading (ISO 17957)，和Resolution (ISO 12233)等，对相关的评测方法、内容等做了详细的规范，能够用于检测成像是否能最真实的还原被摄对象；相比之下，与图像主观评测相关的标准则有较大欠缺，目前仅有的如ITU-R BT.500和ITU-R BT.1788标准，仅对电视系统中的主观测试方法和受测条件进行了规定，并未指出图像主观评估的内容范畴。此外，在移动终端的图像主观评测方面的相关行业标准尚处于空白。

图像主观评测中用于评估图像是否符合可能观看人群的审美属于图像美学评估的内容。一方面，影响最终成像美感的过程和涉及到的美学因素是复杂的，业界对其缺乏统一定义；另一方面，用户在精神及文化上的差异，导致对相同被摄对象存在不同的审美，因而业界在用户关于美的需求侧上也不够了解。而通过确立行业标准，规范美学评估内容和元数据集的结构，借助海量的标注数据驱动美学评估算法，将能够成为解决该问题的重要方向。图像美学评估的实质是量化美感，其主要包括两种方式，一种是对图像的整体美感进行评估，另一种是对图像从多个美学因素上分别评估再综合判断，后者较前者更加科学全面，但对数据集要求更高。

目前已有的图像美学数据集在逻辑结构上缺乏科学性，未能对各类美学因素进行有效划分，不同评估任务之间既缺乏一定的内在联系，又存在因素间的冗余性。同时，可用于训练的美学数据集涵盖的标注范围小，未能对关键美学因素进行系统归纳，由此训练的美学评估模型的量化能力和泛化能力均受限，难以用于实际应用。其主要原因是已有的标准无法规范图像美学的评估内容，以及指导图像美学元数据集的建立。

该标准提出用于构建图像美学元数据集的方法，以角色视角划分图像自产生至美感鉴别过程中所涉及的维度，在逻辑结构上科学严谨；同时对各维度下美学因素进行汇总和归纳，在数据组成上更为细致全面。该标准将从以下几方面发挥重要作用：

（1）能有效指导图像美学元数据集的标注及构建，为图像美学多因素的评估提供数据基础，依此构建数据集并用于驱动美学模型，能够替代普通人工甚至摄影学专家对图像做出全面的美学评价。

（2）能有效提升产品的文化定位和附加属性，例如利用美学评估帮助厂商设计更符合用户需求的美颜类软件；在相机拍照时，对用户在多个维度上进行拍摄指导，辅助用户拍出更美的图像；在数字多媒体运营中，对影像作品进行美感评估后再推荐，以更加贴合当地文化及受众审美等。

（3）该标准作为移动终端计算摄影处理单元子标准，将与后续对于每个美学因素细化形成的一系列标准组成标准体系，弥补图像质量评测行业在图像主观评测方向上的标准欠缺，有效规范行业图像美学评估任务。

