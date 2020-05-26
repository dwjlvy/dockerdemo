

# 基于microsoft/aspnetcore:3.1构建Docker Image
FROM mcr.microsoft.com/dotnet/core/aspnet:3.1-buster-sli
 
# 设置工作路径
WORKDIR /app
 
# 将当前文件夹下的所有文件全部复制到工作目录
COPY *.* ./
 
# 配置环境变量ASPNETCORE_URLS
ENV ASPNETCORE_URLS http://0.0.0.0:5000

# 暴露5000端口
EXPOSE 5000
 
# 执行dotnet GetMachNameWebAPI.dll命令
CMD ["dotnet", "dockertest.dll"]

