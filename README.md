USE [TESTDB]
GO
/****** Object:  Table [dbo].[ImageStore]    Script Date: 13-09-2018 PM 06:20:13 ******/
SET ANSI_NULLS ON
GO
SET QUOTED_IDENTIFIER ON
GO
SET ANSI_PADDING ON
GO
CREATE TABLE [dbo].[ImageStore](
	[ImageId] [int] IDENTITY(1,1) NOT NULL,
	[ImageBase64String] [varchar](max) NULL,
	[CreateDate] [datetime] NULL,
 CONSTRAINT [PK_ImageStore] PRIMARY KEY CLUSTERED 
(
	[ImageId] ASC
)WITH (PAD_INDEX = OFF, STATISTICS_NORECOMPUTE = OFF, IGNORE_DUP_KEY = OFF, ALLOW_ROW_LOCKS = ON, ALLOW_PAGE_LOCKS = ON) ON [PRIMARY]
) ON [PRIMARY] TEXTIMAGE_ON [PRIMARY]

GO
SET ANSI_PADDING OFF
GO
